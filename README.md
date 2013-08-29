PHP Markdown G
==============

A fork of the [PHP Markdown](https://github.com/michelf/php-markdown) parser with Github style.

Differences from PHP Markdown
-----------------------------
This version is based on [PHP Markdown Extra 1.2.7](http://michelf.ca/projects/php-markdown/classic/) by Michel Fortin, released on 11 Apr 2013.  

* Support for Github style fenced code blocks. Wrap code blocks in \`\`\` instead of ~~~.
* Code for third party software removed and global settings moved into class.

How do I use this?
------------------
Download [markdown.php](markdown.php?raw=true) and use it in your programs. Here's an example:

    require_once("markdown.php");
    $markdown = new MarkdownExtra_Parser();
    $html = $markdown->transform($text);

For more information see [original documentation](http://michelf.ca/projects/php-markdown/configuration/).