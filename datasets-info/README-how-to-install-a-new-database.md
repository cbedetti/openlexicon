# How to add a new database #

Let say that your database is named `XXXX` 

1. create a new file `XXXX.json` in `datasets-info`.

You can inspire yourself from the json file associated to the database _Lexique3_

```{json}
  "name": "lexique3",
  "urls": [
    {
      "url": "http://www.lexique.org/databases/Lexique382/Lexique382.tsv",
      "bytes": 25850842 
    }
  ],
  "type": "tsv",
  "tags": ["french", "frequencies"],
  "description": "Lexique382 est une base de données lexicales du français qui fournit pour ~140000 mots du français: les représentations orthographiques et phonémiques, les lemmes associés, la syllabation, la catégorie grammaticale, le genre et le nombre, les fréquences dans un corpus de livres et dans un corpus de sous-titres de filems, etc.",
  "readme": "http://chrplr.github.io/openlexicon/datasets-info/Lexique382/README.md"
}
```

2. Optionaly, you can create a subfolder with more info about the database in `datasets-info`

3. If the dataset is not yet on the Internet, you need to put it on a server somewhere.


For example, for <www.lexique.org> maintainers:


* Connect to the server and go to the database directory 

    cd /var/www/databases

* Create a folder for the newdatabase:
   * add there the relevant files (csv, tcsv, xlsx, zip, ...)
   * create a `database2rdata.R` script in this folder and run it to generate a RData file containing the database. 
   
* Go to you fork of <http://github.com/chrplr/openlexicon/datasets-info> and add some documentation --- at a minimum a README.md file) describing the database -- and issue a pull request.

* Optionaly, if you want to make the database accessible in openlexique:
   * Add a link to the `.RData` file on the server and run:  
   
           sudo systemctl restart shiny-server.service
   
   * Modify the [openlexicon apps](http://github.com/chrplr/openlexicon/apps) that will use this database (or issue a pull request).
   * Connect to the server and run: 
   
        cd ~chrplr/shiny-server
        git pull
--

Back to [OpenLexicon](https://chrplr.github.com/openlexicon)


Time-stamp: <2019-04-25 09:07:50 christophe@pallier.org>