File-Parsing
============

A project to parse a PDF invoice and extract the items contained in the invoice as well as additional meta data.


#### Installation

To get started:

1. Install [node.js](http://nodejs.org/download).
1. Install [Mocha](http://visionmedia.github.io/mocha/):

    $ npm install -g mocha

1. In this directory, run "$ npm install" then install [pdftotext](http://linuxappfinder.com/package/poppler-utils).

#### Testing

Simply run [Mocha](http://visionmedia.github.io/mocha/). The easiest way to do this is via npm:

    $ npm test

#### Getting Started

After running the tests to see what's failing, look at parseText function in index.js. Try to take the text 
that you're given and identify invoice line items, then add those items to the results.items array. To try
things out more interactively, open a node REPL, read the sample text file in (via 
[fs.readFileSync](http://nodejs.org/api/fs.html#fs_fs_readfilesync_filename_options)) then try various 
[regular expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions).

Only consider the input file as set in stone. Everything else, including the tests, can be changed if you
think it will improve the results.

Have Fun.
