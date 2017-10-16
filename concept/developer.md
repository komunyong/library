# Bookmark for developer role

## Video Based Tutorial

* [Laracast](https://laracasts.com/): PHP Laravel Framework, Vue and Design Pattern for MVP.
* [Datacamp](https://www.datacamp.com/) - Video tutorials for data scientist.

## Text Based Tutorial (Blog post / Github)

* [Series] [R Beginner](http://www.cyclismo.org/tutorial/R/index.html)
* [Series] [Google Code Lab](https://codelabs.developers.google.com/)

## Online Tools

* [Cloudcraft](https://cloudcraft.co/) - AWS 3D Online Architecture Diagram
* [Recordit](http://www.recordit.co/) - Record screen as GIF image to make easy tutorial.


## REPL (Read eval print loop)

is shell for run programming language directly

## Semantic Versioning

For versioning your software (MAJOR.MINOR.PATCH)

* MAJOR version when you make **incompatible API changes**,
* MINOR version when you add functionality in a **backwards-compatible** manner, and
* PATCH version when you make **backwards-compatible bug fixes**.

REF: [semver](http://semver.org/)


## YAML Syntax

human-readable data serialize language that mostly used for configuration file. Be alternate choices with JSON and XML.

```yaml
receipt: Oz-Ware Purchase Invoice
date: 2012-08-06
customer:
    first_name: Dorothy
    family_name: Gale

items:
  - part_no: A4786
    descrip: Water Bucket (Filled)
    price: 1.47
    quantity: 4

  - part_no: E1628
    descrip: High Heeled "Ruby" Slippers
    size: 8
    price: 133.7
    quantity: 1

bill-to:  &id001
  street: |
          123 Tornado Alley
          Suite 16
  city:   East Centerville
  state:  KS

ship-to:  *id001

specialDelivery:  >
    Follow the Yellow Brick
    Road to the Emerald City.
    Pay no attention to the
    man behind the curtain.
```

REF: [YAML](https://en.wikipedia.org/wiki/YAML)


## CORS (Cross-origin resource sharing)

For security reason that domain will only allow request from its own domain only as default. In short, browser not allow fire request to different domain.

* PUT, DELETE or send content type as application/json, required preflight request.

REF: 
* [How to enable CORS in server](https://enable-cors.org/server.html)
* [Same origin policy about CORS](https://en.wikipedia.org/wiki/Same-origin_policy#Origin_determination_rules)
* [Chrome extension](https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi?hl=en) to allow-origin as * to develop in local

## UUID/GUID
Universally Unique Identifier / globally unique identifier is 128-bit number used to identify information in computer systems, mostly required unique in huge system. MySQL uses UUID version 1 which is a 128-bit number represented by a utf8 string of five hexadecimal numbers (58e0a7d7–eebc–11d8-9669-0800200c9a66)
* The first three group numbers are generated from a timestamp.
* The fourth group number preserves temporal uniqueness in case the timestamp value loses monotonicity (for example, due to daylight saving time).
* The fifth group number is an IEEE 802 node number that provides spatial uniqueness. A random number is substituted if the latter is not available (for example, because the host computer has no Ethernet card, or we do not know how to find the hardware address of an interface on your operating system). In this case, spatial uniqueness cannot be guaranteed. Nevertheless, a collision should have very low probability.

REF:

* [Store UUID Optimized Way](https://www.percona.com/blog/2014/12/19/store-uuid-optimized-way/)
* [Postgres UUID Usage](https://www.postgresql.org/docs/9.4/static/datatype-uuid.html)
* [MySQL UUID Usage](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_uuid)

## Compile concept - just-in-time (JIT) and ahead-of-time (AOT)

* JIT is compile part of code to executable file only part that need to run, install fast but slow usage (require to compile a little bit before execute)
* AOT is compile all source code to executable file at first time (installing app), install slow but fast usage

## Why keep SQL out from source code

* Easy to track when need to modify
* New developer can easy to learn DB Structure
* Easy to maintain when change schema
* Migrate to another framework easily

 REF: [Keep SQL out of code](http://www.javapractices.com/topic/TopicAction.do?Id=105)

## Log / Search Platform

[Node JS Logging](https://blog.risingstack.com/node-js-logging-tutorial/)
[Centralized Log in Distributed System](https://www.elastic.co/)
[Centralized Log with AWS Solution](https://aws.amazon.com/answers/logging/centralized-logging/)

## Programming Paradigm

* Reactive
  * [Reactive Programming](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)
  * [ReactiveX](http://reactivex.io/)

## Design Pattern

* Component Based
  * [BEM - Block Element Modifier](https://en.bem.info/methodology/)
  * [React JS](https://reactjs.org/)

* MVC (Model View Controller) - have Controller to routing in your app and be middleware between Model and View, Model is connect direct with Database layer, View is display output to user (eg. HTML and front-end)
  * [MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller)
  * [ASP.NET CORE - MVC Framework](https://docs.microsoft.com/th-th/aspnet/core/)
  * [PHP Laravel - MVC Framework](https://laravel.com/)

* Component-based MVC
  * [Angular JS](https://angularjs.org/)

## Editor Modify

### VSCode nice packages

* One Dark Pro Theme
* VSCode Great Icons
* To Do Tasks
* ESLint
* Gitlens - for blaming people
* ES7 Snippet
* markdownlint

## Terminal Modify

* [cmder](http://cmder.net/) - Portable console emulator for Windows
* [zsh](http://www.zsh.org/) - shell designed for interactive use, although it is also a powerful scripting language.
* [oh-my-zsh](http://ohmyz.sh/)