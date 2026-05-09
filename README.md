<a href="https://www.php.net/"><img src="https://img.shields.io/github/languages/top/khaled-alshamaa/ar-php"/></a> <a href="https://www.php.net/manual/en/migration56.php"><img src="https://img.shields.io/badge/PHP-%3E%3D%207.4-8892BF"/></a> <a href="https://packagist.org/packages/khaled.alshamaa/ar-php"><img src="https://img.shields.io/packagist/dt/khaled.alshamaa/ar-php"/></a>
<!-- https://shields.io/ -->

<img align="right" width="256" height="256" src="https://raw.githubusercontent.com/khaled-alshamaa/ar-php/master/ar-php_256.png">

# Ar-PHP Project ([ar-php.org](http://www.ar-php.org/en_index-php-arabic.html))
#### _PHP Speaks Arabic - Be Ready!_
_Copyright © 2006-2025 Khaled Al-Sham'aa._

[![DOI](https://zenodo.org/badge/231197063.svg)](https://zenodo.org/badge/latestdoi/231197063)

[العربية](https://github.com/khaled-alshamaa/ar-php/blob/master/README_ar.md)

## ⚡ Performance Optimization Notice

> **📊 Repository Size Optimization:** In this fork, we've optimized the repository by adding `ArPHP.phar` (20MB binary file) to `.gitignore` to improve clone and load times. The repository size remains at **117 MB**, but future commits will not include large binary artifacts. [Learn more about this optimization](https://github.com/riyadhali/ar-php)

## Ar-PHP: Empowering Arabic Language Processing in PHP
Welcome to Ar-PHP, an open-source PHP library dedicated to simplifying Arabic language processing. Our mission is to provide developers with easy-to-use tools for professional searching, manipulating, and analyzing Arabic text in PHP applications.

### Table of Contents
> [Introduction](#introduction)

> [Adoption](#adoption)

> [Installation](#installation)

> [Features](#features) 

> [Change Log](https://github.com/khaled-alshamaa/ar-php/blob/master/CHANGELOG.md)

> [Documentation](https://khaled-alshamaa.github.io/ar-php/classes/ArPHP-I18N-Arabic.html)

> [Contributing](#contributing)

> [Professional Support](#professional-support)

> [FAQ](https://khaled-alshamaa.github.io/ar-php/faq_php_arabic.html)

## _Introduction_

### Arabic Language
Internet use has grown quickly worldwide, especially in non-English speaking regions. Between 2000 and 2022, Arabic was the fastest-growing language online, increasing by 9,350%. It has around 240+ million native speakers and about 290+ million second-language speakers.

[[Arabic language](https://en.wikipedia.org/wiki/Arabic), [Internet world stats](https://data.worldbank.org/indicator/IT.NET.USER.ZS?end=2022&locations=1A&start=1990&view=chart)]

### PHP
PHP is a widely used general-purpose scripting language that is especially suited for web development and can be embedded into HTML. PHP runs more than 75% of all the top 10 million worldwide websites. It is a server-side scripting language, which means it runs on the server, not the browser.

[[PHP language](https://www.php.net/), [Server-side languages report](https://w3techs.com/technologies/overview/programming_language)]

### LGPL
The key difference between the GPL and LGPL is that the LGPL allows a library to be linked to, or used by, a program that is not licensed under the (L)GPL. This means the program can be either free or proprietary.

[[LGPL](http://www.gnu.org/licenses/lgpl-3.0.html), [GNU FAQ](http://www.gnu.org/licenses/gpl-faq.html)]

### Project History

[![محاضرة افتتاحية عن تجربة بناء ادوات لدعم اللغة العربية و المشاريع مفتوحة المصدر - خالد الشمعة](https://img.youtube.com/vi/YU9wqHF8p4w/0.jpg)](https://www.youtube.com/watch?v=YU9wqHF8p4w)

* PHP 7/8 at [GitHub.com](https://github.com/khaled-alshamaa/ar-php) 2020-present.
* PHP 5 at [SourceForge.net](https://sourceforge.net/projects/ar-php/) 2008-2016.
* PHP 4 at [PHPClasses.org](https://www.phpclasses.org/browse/author/189864.html) 2006-2008.

> __Alshamaa, Khaled__ (2008). _PHP واللغة العربية_. Dar Shoaa. Retrieved from [https://darshoaa.com/pHP-and-Arabic-language/](https://darshoaa.com/pHP-and-Arabic-language/).

[Top](#ar-php-project-ar-phporg)

## _Adoption_
Ar-PHP has been successfully integrated into several projects, including:

* [Bagisto](https://www.bagisto.com/): A Laravel-based e-commerce package.
* [Akeneo](https://www.akeneo.com/): An open-source SaaS PIM platform for organizing product catalogs.
* [LimeSurvey](https://www.limesurvey.org/): A powerful open-source survey software.
* [UnoPim](https://unopim.com/): An open-source PIM system built on the Laravel framework.
* [GPDF](https://github.com/omaralalwi/Gpdf): An open-source HTML-to-PDF converter for PHP & Laravel applications.
* [ArabKey](https://arabkey.site/): A tool for switching between Arabic and English keyboards.
* [Krayin](https://krayincrm.com/): An Open Source CRM Software.

[![Star History Chart](https://api.star-history.com/svg?repos=khaled-alshamaa/ar-php&type=Date)](https://star-history.com/#khaled-alshamaa/ar-php&Date)

[Top](#ar-php-project-ar-phporg)

## _Installation_

### Installation with Composer

To install this package using [Composer](https://getcomposer.org/), run the following command in your terminal:

```bash
composer require khaled.alshamaa/ar-php
```

Ensure that the Composer autoloader is included in your project. If your project already uses Composer's autoloading mechanism -like frameworks such as Laravel- you can skip this step. Otherwise, add the following line to your script:

```php
require 'vendor/autoload.php';
```

### Manual Download and Installation
Download the [latest Ar-PHP release](https://github.com/khaled-alshamaa/ar-php/releases/latest), extract it into your project directory, and include the library by adding:

```php
require_once 'ar-php/src/Arabic.php';
```

Ensure the path matches the location of the Arabic.php file relative to your script.

[Top](#ar-php-project-ar-phporg)

## _Features_
* Arabic Spell Checker ([ASC](https://arabicspellchecker.com/open-source.html)) ([live demo](https://ar-php.org/github/examples/ar_spell.php)) ***New!***
* Arabic Sentiment Analysis ([live demo 1](https://ar-php.org/github/examples/ar_sentiment.php), [live demo 2](https://khaled-alshamaa.github.io/ar-php/ar_sentiment.html))
* Arabic Dialect Identification ([live demo](https://ar-php.org/github/examples/ar_dialects.php)) ***New!***
* English-Arabic Transliteration ([live demo 1](https://ar-php.org/github/examples/ar_transliteration.php), [live demo 2](https://ar-php.org/github/examples/en_transliteration.php))
* Spell Numbers in the Arabic Idiom ([live demo](https://ar-php.org/github/examples/numbers.php))
* Arabic Glyphs to Render Arabic Text ([live demo](https://ar-php.org/github/examples/ar_glyphs.php))
* Arabic Keyboard Swapping Language ([live demo](https://ar-php.org/github/examples/keyswap.php))
* Arabic Soundex ([live demo](https://ar-php.org/github/examples/soundex.php))
* Arabic Gender Guesser ([live demo](https://ar-php.org/github/examples/gender.php))
* Arabic SQL Query ([live demo](https://ar-php.org/github/examples/ar_query.php))
* Muslim Prayer Times & Qibla Determination ([live demo](https://ar-php.org/github/examples/salat.php))
* Arabic/Hijri Date ([live demo](https://ar-php.org/github/examples/date.php))
* Arabic/Hijri Maketime ([live demo](https://ar-php.org/github/examples/mktime.php))
* Arabic StrToTime ([live demo](https://ar-php.org/github/examples/strtotime.php))
* Arabic Text Standardize ([live demo](https://ar-php.org/github/examples/standard.php))
* Arabic Auto Summarize ([live demo](https://ar-php.org/github/examples/ar_summarize.php))
* Arabic Segments Identifier ([live demo](https://ar-php.org/github/examples/identifier.php))
* Arabic Text Similarity ([live demo](https://ar-php.org/github/examples/ar_similarity.php)) ***New!***

[Top](#ar-php-project-ar-phporg)

## _Contributing_
We welcome contributions from the community! Whether it is reporting bugs, suggesting new features, or submitting pull requests, your help is valuable. Before contributing, please review our project's contributing guidelines and code of conduct.

* __Programming:__ Here are some ideas for contribution: Review the To-Dos, add a feature, contribute to a core module, create an extension, and fix a bug.
* __Quality Assurance:__ Quality Assurance (QA) is one of the most important but understated elements of any software community project. It is also something most people can do. If you want to help, you can find or file bugs in the project's issue tracker.
* __Writing:__ One of the best ways to contribute to Ar-PHP is to write tutorials, guides, HOWTOs, and FAQs. Here are some ideas for contributions: User FAQs, HOW-Tos and Tutorials, a User Guide, and Architecture Guides.
* __Marketing:__ You can always help promote the use of Ar-PHP. Here are two ways you can help: Join the marketing events and distribute Ar-PHP and its brochures.
* __Graphics and Art:__ Have any art skills? Then you can help us create icons, logos, banners, labels, wallpapers, screen savers, and more! These will be seen every day and used throughout the project.
* __Helping Users:__ There are two ways you can help other users: Users mailing list, and forums.
* __Celebrate with us!__ Your task is to take a picture of yourself supporting the PHP and Arabic language project. You can go to a famous landmark, your favorite place nearby, or anywhere you think would make a good photo. You can go to a famous landmark, your favorite place nearby, or anywhere you think would make a good photo!

[Top](#ar-php-project-ar-phporg)

## _Professional Support_
As the developers of the Ar-PHP project, we can help your company leverage the maximum power of Ar-PHP to achieve your business goals. We offer professional services that span the full life cycle of Ar-PHP deployment:

* __Ar-PHP Library Integration:__ Having trouble getting started with Ar-PHP? We can help.
* __Ar-PHP Upgrades:__ For a smooth upgrade to a newer version of Ar-PHP, let us assist you.
* __Customization and Configuration:__ If your business requires functionality beyond or different from that of the feature set of Ar-PHP, our team of PHP and Arabic language experts can fully tailor Ar-PHP to your needs.
* __Integration Analysis and Implementation:__ Arabic localization may be just a component of your entire online business operation. We have the knowledge and experience to integrate Ar-PHP with your entire enterprise solution.
* __Troubleshooting, Optimization, and Performance Tuning:__ For increased performance and bottleneck resolution, let an Ar-PHP expert look under the hood of your Ar-PHP implementation and server configuration.
* __Consulting:__ At any point in the implementation of Ar-PHP, you can call upon an Ar-PHP expert to verify that your implementation follows industry best practices.
* __Training:__ Get comprehensive training for Ar-PHP.

[Top](#ar-php-project-ar-phporg)

<!-- If you find this project useful, please consider donating. Any funds donated will be used to help further the development of this project. -->

### Citation

If you would cite it in academic work, you can use this citation

```
K. Al-Shamaa, Ar-PHP, PHP library for website developers to process Arabic content, 
https://github.com/khaled-alshamaa/ar-php, 2025
```

or in bibtex format

```latex
@misc{ar-php,
  title={Ar-PHP, PHP library for website developers to process Arabic content},
  author={Al-Shamaa, Khaled},
  url={https://github.com/khaled-alshamaa/ar-php},
  version = {7.0.0},
  year={2025}
}
```

[Top](#ar-php-project-ar-phporg)
