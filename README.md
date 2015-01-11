## Parsedown

Better Markdown Parser in PHP

[[ demo ]](http://parsedown.org/demo)

### Features

* [Fast](http://parsedown.org/speed)
* [Consistent](http://parsedown.org/consistency)
* [GitHub flavored](https://help.github.com/articles/github-flavored-markdown)
* [Tested](http://parsedown.org/tests/) in PHP 5.2, 5.3, 5.4, 5.5, 5.6 and [hhvm](http://www.hhvm.com/)
* Extensible
* [Markdown Extra extension](https://github.com/erusev/parsedown-extra)
* [JavaScript port](https://github.com/hkdobrev/parsedown.js) under development

### Installation

Include `Parsedown.php` or install [the composer package](https://packagist.org/packages/erusev/parsedown).

### Example

``` php
$Parsedown = new Parsedown();

echo $Parsedown->text('Hello _Parsedown_!'); # prints: <p>Hello <em>Parsedown</em>!</p>
```

More examples in [the wiki](https://github.com/erusev/parsedown/wiki/Usage) and in [this video tutorial](http://youtu.be/wYZBY8DEikI).

### Questions

**How does Parsedown work?**<br/>
It tries to read Markdown like a human. First, it looks at the lines. It’s interested in how the lines start. This helps it recognise blocks. It knows, for example, that if a line start with a `-` then it perhaps belong to a list. Once it recognises the blocks, it continues to the content. As it reads, it watches out for special characters. This helps it recognise inline elements (or inlines).

**Why doesn’t Parsedown use namespaces?**<br/>
It'd mean no support for PHP 5.2. Would it be worth it?

**Is Parsedown compliant with CommonMark?**<br/>
The majority of the CommonMark tests pass. Most of the tests that don't pass deal with cases that are quite extreme. Yet, we are working on them. As CommonMark matures, compliance should improve.

**Who uses Parsedown?**<br/>
[phpDocumentor](http://www.phpdoc.org/), [October CMS](http://octobercms.com/), [Bolt CMS](http://bolt.cm/), [Kirby CMS](http://getkirby.com/), [Grav CMS](http://getgrav.org/),  [RaspberryPi.org](http://www.raspberrypi.org/) and [more](https://www.versioneye.com/php/erusev:parsedown/references).

**How can I help?**<br/>
Use the project, tell friends about it and if you feel generous, [donate some money](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=528P3NZQMP8N2).
