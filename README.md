Transliterator
=======================

Transliterator transliterate into Latin characters of Cyrillic characters.
Use the [international standard ISO 9](http://en.wikipedia.org/wiki/ISO_9).

Transliterator can be used as either a widget or a controller filter.

Usage as a class:
------------
~~~
$translator = new Transliterator;
$translator->standard = Transliterator::GOST_779A;
$text = $translator->transliterate($text);
~~~

Usage as validation rule:
------------
~~~
array('text', 'filter', 'filter' => array($obj = new Transliterator, 'transliterate')),
~~~