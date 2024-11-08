<div align="center">

<!-- title -->

<!--lint ignore no-dead-urls-->

# Awesome Hledger [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) 

<!-- subtitle -->

Guides and tools for [hledger](https://hledger.org).

<!-- image -->

<a href="https://hledger.org" target="_blank" rel="noopener noreferrer">
  <img src="https://hledger.org/images/coins2-248.png" />
</a>

<!-- description -->

Manage your finances using a plain text file

</div>

## Table of Content
<!-- TOC -->
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Text Editor Tools](#text-editor-tools)
- [TUI - Terminal User Interface to view, add and manage journal files](#tui---terminal-user-interface-to-view-add-and-manage-journal-files)
- [GUI - Web, Desktop and Mobile user interfaces](#gui---web-desktop-and-mobile-user-interfaces)
- [Add/Edit Transactions](#addedit-transactions)
- [Import Transactions](#import-transactions)
- [Report](#report)
- [Price Fetching](#price-fetching)
- [Guides, Tutorial and Blog Posts](#guides-tutorial-and-blog-posts)
- [Videos](#videos)
- [Related Tools](#related-tools)
- [Community](#community)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Text Editor Tools

Since hledger is based on a plain text journal file, a text editor is the main tool to edit transactions. These extensions can be added to the text editors to make life easier as explained [here](https://hledger.org/editors.html).

- [Emacs ledger-mode](https://github.com/ledger/ledger-mode) - Most used and maintained helper mode for hledger and Ledger files, but not 100% compatible with hledger.
- [Emacs hledger-mode](https://github.com/narendraj9/hledger-mode) - An alternative to ledger-mode, written specifically for hledger. Has some different features. 
- [Emacs flycheck-hledger](https://github.com/DamienCassou/flycheck-hledger) - Provides realtime indication of problems in your journal. Can be combined with ledger-mode or hledger-mode.
- [Vim vim-ledger](https://github.com/ledger/vim-ledger) - Vim plugin compatible with *ledger* and *hledger*.
- [Vim hledger-vim](https://github.com/anekos/hledger-vim) - Alternative to *vim-ledger*.
- [Vim timedot-vim](https://github.com/linuxcaffe/timedot-vim) - timedot-vim is a vim-plugin to enhance working with hledger timedot files.
- [VS Code hledger-vscode](https://github.com/mhansen/hledger-vscode) - Language support for hledger in VS Code

## TUI - Terminal User Interface to view, add and manage journal files

Interactive apps on terminal to navigate the transactions using menus, dialogs and reports without the need to use multiple command-line options.

- [hledger-ui](https://hledger.org/1.29/hledger-ui.html "hledger-ui") - Official terminal interface for hledger.
- [puffin](https://github.com/siddhantac/puffin) - A bubbletea based TUI to manage personal finances using hledger

## GUI - Web, Desktop and Mobile user interfaces

Beautiful and graphical applications to manage journal files

- [hledger-web](https://hledger.org/1.29/hledger-web.html) - Official web interface for hledger.
- [MoLe](https://mole.ktnx.net/) - Android front end to hledger-web

## Add/Edit Transactions

Even complex transactions become simple and convenient to add with these tools.

- [hledger add](https://hledger.org/1.29/hledger.html#add) - Official interactive command-line tool to add transactions.
- [hledger-iadd](https://github.com/hpdeifel/hledger-iadd) - Very convenient tool to add transactions to hledger journal.
- [hledger-edit](https://gitlab.com/nobodyinperson/hledger-utils#hledger-edit-editing-hledger-transactions-in-your-editor) - Edit hledger transactions in your $EDITOR limited to the result of a query.
- [hledger-lots](https://edkedk99.github.io/hledger-lots/) - Add transactions involving buying and selling commodities with prices to for automatic lot management.
- [obsidian_hledger](https://github.com/bzimor/obsidian_hledger) - Add transactions using Obsidian.

## Import Transactions

Bring transactions from other sources to hledger's format.

- [hledger (Built-in)](https://hledger.org/1.29/hledger.html#csv) - Built-in hledger's command to convert csv files.
- [hledger-flow](https://github.com/apauley/hledger-flow) - Guided hledger workflow to import transactions.
- [ledger-autosync](https://gitlab.com/egh/ledger-autosync) - Import OFX file to hledger.
- [invoice2data](https://github.com/invoice-x/invoice2data) - Import transactions from pdf invoices.

## Report

The ultimate reason to maintain a journal file is to extract information. Use these tools to process and visualize the data.

- [hledger-plot](https://gitlab.com/nobodyinperson/hledger-utils#hledger-plot-plotting-charts-of-hledger-querieshledger-plot) - Plot chart of hledger queries.
- [hledger-args](https://github.com/edkedk99/hledger-args) - replacement for hledger command file using custom directives inside the journal file. Also provides an interactive report with placeholders to generate prompts.
- [hledger2psql](https://github.com/edkedk99/hledger2psql) - Export a hledger journal file to a postgresql database to be used in data visualization software. Included docker-compose file for *Apache Superset*.
- [hledger-lots](https://edkedk99.github.io/hledger-lots/) - View financial indicator including market price, profit and XIRR for one commodity or all commodities in a tabular form.
- [hledger-forecast](https://github.com/olimorris/hledger-forecast) - Use a CSV or Yaml file for easier forecasting with hledger. Adds functionality for future cost rises (e.g. inflation) and the automatic tracking of planned transactions.

## Price Fetching

- [pricehist](https://gitlab.com/chrisberkhout/pricehist) - Download price history from multiple sources and output to multiple formats, including hledger price directive.
- [hledger-stockquotes](https://github.com/prikhi/hledger-stockquotes#readme) - Read your journal and and try to download price directives for all non USD declared commodities.
- [hledger-lots](https://edkedk99.github.io/hledger-lots/) - Create automatic lots without subaccounts and tags and download prices from declared accounts in the journal with a specific [tag](https://hledger.org/1.29/hledger.html#tags)


## Guides, Tutorial and Blog Posts

- [contrib-resources](https://github.com/edkedk99/awesome-hledger/tree/master/contrib-resources) - Place with resources about hledger in /awesome-hledger/ where any user can contribute with tutorials, articles, tips, etc.
- [gizra.com](https://www.gizra.com/content/plain-text-accounting-hledger/) - Great introduction to hledger.
- [Barracudo Blog Post](https://memo.barrucadu.co.uk/personal-finance.html) - Lengthy discussion of a hledger personal usage.
- [functional-finance-hledger](https://pauley.org.za/functional-finance-hledger/) - Slides on a hledger workflow based on importing csv files
- [hledger github topic](https://github.com/topics/hledger?o=desc&s=updated) - Github topics page for hledger.
- [hledgerfans](https://hledgerfan.com/) - Blog posts about hledger.

## Videos

- [Inside hledger](https://www.youtube.com/watch?v=6PKmZSHxu0c) - Discussion of the source code with a general discussion about hledger.
- [Floss Weekly](https://www.youtube.com/watch?v=Xjl-wVJcYpE) - General discussion about hledger.
- [Glenn Ramsey](https://www.youtube.com/watch?v=lazZwTmAEHs) - Introduction to hledger focused on invoice generation and csv import.

## Related Tools

These tools are not made for hledger, but they provide useful workflows to maintain journal files.

- [Tabula](https://github.com/tabulapdf/tabula) - Extract data from tables in a pdf file to import to hledger.
- [csvkit](https://csvkit.readthedocs.io) - Convert to csv and do operating like cut, grep, sort, join, stack, etc.
- [GNU Make](https://www.gnu.org/software/make/) - Set multiple conversions, import and other operations for you ledger files.
- [hledger-fmt](https://github.com/mondeja/hledger-fmt) - Format hledger's journal files.
- [watchexec](https://github.com/watchexec/watchexec) - Automatically run a hledger command when the journal changes. Available in most linux distributions.
- [entr](https://github.com/eradman/entr) - Alternative to [watchexec](https://github.com/watchexec/watchexec)

## Community

Places to ask question about hledger and accounting in general

- [contrib-resources](https://github.com/edkedk99/awesome-hledger/tree/master/contrib-resources) - Place with resources about hledger in /awesome-hledger/ where any user can contribute with tutorials, articles, tips, etc.
- [Reddit](https://www.reddit.com/r/plaintextaccounting/) - Plain Text Accounting with hledger and others ledger-like software.
- [Matrix Chat](http://matrix.hledger.org/) - Matrix Chat room using [element](https://element.io/) chat client.
- [Libera IRC](http://irc.hledger.org/) - Same chat room as the matrix, but using IRC.




<!-- END CONTENT -->

<!-- omit in toc -->
## Contributing

[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors

[Thanks goes to these contributors](https://github.com/edkedk99/awesome-hledger/graphs/contributors)!
