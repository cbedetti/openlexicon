OpenLexicon: Easy access to lexical databases
=============================================

At OpenLexicon, you will find:

1.  a [directory of lexical databases](datasets-info/README.md)
2.  [scripts](https://github.com/chrplr/openlexicon/tree/master/scripts)
    to query, manipulate or create lexical databases.
3.  [apps](https://github.com/chrplr/openlexicon/tree/master/apps/) to
    create dynamic graphical interfaces to the lexical databases.
4.  [documents](https://github.com/chrplr/openlexicon/tree/master/documents/)
    of interest related to the processing of lexical resources.

-   To add a new dataset, add a `.json` in `datasets-info/`; check out
    [How-to-install-a-new-dataset](datasets-info/README-how-to-install-a-new-database.md).
-   Some of the apps provide the infrastructure of
    <http://www.lexique.org> where many of lexical databases are hosted
    and can be queried on-line --- check out, for example,
    <http://www.lexique.org/shiny/openlexicon>.
-   To automatically download datasets, you can use
    [fetch\_datasets.R](https://raw.githubusercontent.com/chrplr/openlexicon/master/datasets-info/fetch_datasets.R)

### Contributing

Everybody is warmly encouraged to contribute, by adding a database, an
app, or a script. First, check out Lexique's google-group at
<https://groups.google.com/forum/#!forum/lexiqueorg>. You can then
contact `christophe@pallier.org` and `boris.new@gmail.com` privately,
or, *much better*, fork the
[openlexicon](https://github.com/chrplr/openlexicon) repository (see
[How to fork a repo](https://help.github.com/en/articles/fork-a-repo))
and issue a pull request (see [Creating a pull request from a
fork](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork)).

Check out the [TODO list](TODO.md)

### Crediting

Most databases have associated publications listed in their respective
`README` files. They must be cited in any derivative work! The same goes
for some of the scripts (read their documentation for instructions).

If needed, you can cite this repository as:

-   Pallier, Christophe & New, Boris (2019\*\* Openlexicon, GitHub
    repository, <https://github.com/chrplr/openlexicon>

------------------------------------------------------------------------

**For maintainers:**

-   [Server installation](README-server-installation.md)

### License

The files in this repository are distributed under a CC BY-SA 4.0
LICENSE (see <https://creativecommons.org/licenses/by-sa/4.0/>).

------------------------------------------------------------------------

Time-stamp: \<2019-05-01 09:48:32 christophe\@pallier.org\>
