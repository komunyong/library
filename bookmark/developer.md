# Bookmark for developer role

### Video learning

* [Laracast](https://laracasts.com/): PHP Laravel Framework, Vue and Design Pattern for MVP.

### REPL (Read eval print loop)

is shell for run programming language directly

### Semantic Versioning

For versioning your software (MAJOR.MINOR.PATCH)

* MAJOR version when you make **incompatible API changes**,
* MINOR version when you add functionality in a **backwards-compatible** manner, and
* PATCH version when you make **backwards-compatible bug fixes**.

REF: [semver](http://semver.org/)

### YAML Syntax

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

### CORS (Cross-origin resource sharing)

For security reason that domain will only allow request from its own domain only as default. In short, browser not allow fire request to different domain.

* PUT, DELETE or send content type as application/json, required preflight request.

* [How to enable CORS in server](https://enable-cors.org/server.html)
* [Same origin policy about CORS](https://en.wikipedia.org/wiki/Same-origin_policy#Origin_determination_rules)
* [Chrome extension](https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi?hl=en) to allow-origin as * to develop in local