Installing and upgrading
========================

Installation is the same as for most WordPress plugins,
but note that you can get extra features by installing other plugins,
and upgrading requires some changes whenever the major version number increases
(e.g. 2.x.x to 3.x.x).

Install
-------

1. Install the plugin in `the usual way`_ by using your site's plugin manager.
   For Entity Relationship Diagram support, also install the `TFO Graphviz`_ plugin (``tfo-graphviz``).
2. Browse to the Tabulate overview page via the main menu in the WordPress admin area.
3. Create some tables. Alternatively, you can use a tool such as `PHPmyAdmin`_ or `MySQL Workbench`_.

.. _`the usual way`: http://codex.wordpress.org/Managing_Plugins#Installing_Plugins
.. _`TFO Graphviz`: https://wordpress.org/plugins/tfo-graphviz/
.. _`PHPmyAdmin`: http://www.phpmyadmin.net
.. _`MySQL Workbench`: http://mysqlworkbench.org/

Upgrade
-------

When upgrading, please *deactivate* and then *reactivate* the plugin.
This will ensure that all required database updates are carried out
(but will avoid the overhead of checking whether these are required on every Tabulate page load).

Earlier versions of Tabulate required the REST API plugin
(either version 1, ``json-rest-api``; or version 2, ``rest-api``)
as the API was moved into core WordPress.
You can remove these plugins if you have them.

Tabulate can be deactivated and reactivated without losing any data;
if uninstalled, it will remove everything that it's added
(but you will be warned before this happens, don't worry).

None of your custom database tables are modified
during upgrade, activation, deactivation, or uninstallation.
