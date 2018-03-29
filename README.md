# Merriam.IO Community

This repository holds the content of Merriam.IO APIs access libraries

* [Homepage](https://merriam.github.io/)
* [API documentation](#api-documentation)

It has following client libraries with its tremendous features at a General Availability(#versioning) (GA) quality level:

* [Node](https://github.io/MerriamIO/merriam-node) (GA)
* [Angular2](https://github.io/MerriamIO/merriam-angular2) (GA)
* [Python](https://github.io/MerriamIO/merriam-node) (GA)
* [PHP](https://github.io/MerriamIO/merriam-php) (GA)
* [Java](https://github.io/MerriamIO/merriam-java) (GA)
* [Ruby](https://github.io/MerriamIO/merriam-node) (GA)

# api-documentation

Merriam.IO Client Library for REST APIs

Register yourself and get your `key` from [here](https://merriam.io) for authentication

List Languages

```
curl -X GET -H "Accept:application/json" https://merriam.io/api/v1/languages.json?key=<your-api-key>

[{"code":"af","name":"Afrikaans"},{"code":"sq","name":"Albanian"},{"code":"am","name":"Amharic"},{"code":"ar","name":"Arabic"},{"code":"hy","name":"Armenian"},{"code":"az","name":"Azerbaijani"},{"code":"eu","name":"Basque"},{"code":"be","name":"Belarusian"},{"code":"bn","name":"Bengali"},{"code":"bs","name":"Bosnian"},{"code":"bg","name":"Bulgarian"},{"code":"ca","name":"Catalan"},{"code":"ceb","name":"Cebuano"},{"code":"ny","name":"Chichewa"},{"code":"zh","name":"Chinese (Simplified)"},{"code":"zh-TW","name":"Chinese (Traditional)"},{"code":"co","name":"Corsican"},{"code":"hr","name":"Croatian"},{"code":"cs","name":"Czech"},{"code":"da","name":"Danish"},{"code":"nl","name":"Dutch"},{"code":"en","name":"English"},{"code":"eo","name":"Esperanto"},{"code":"et","name":"Estonian"},{"code":"tl","name":"Filipino"},{"code":"fi","name":"Finnish"},{"code":"fr","name":"French"},{"code":"fy","name":"Frisian"},{"code":"gl","name":"Galician"},{"code":"ka","name":"Georgian"},{"code":"de","name":"German"},{"code":"el","name":"Greek"},{"code":"gu","name":"Gujarati"},{"code":"ht","name":"Haitian Creole"},{"code":"ha","name":"Hausa"},{"code":"haw","name":"Hawaiian"},{"code":"iw","name":"Hebrew"},{"code":"hi","name":"Hindi"},{"code":"hmn","name":"Hmong"},{"code":"hu","name":"Hungarian"},{"code":"is","name":"Icelandic"},{"code":"ig","name":"Igbo"},{"code":"id","name":"Indonesian"},{"code":"ga","name":"Irish"},{"code":"it","name":"Italian"},{"code":"ja","name":"Japanese"},{"code":"jw","name":"Javanese"},{"code":"kn","name":"Kannada"},{"code":"kk","name":"Kazakh"},{"code":"km","name":"Khmer"},{"code":"ko","name":"Korean"},{"code":"ku","name":"Kurdish (Kurmanji)"},{"code":"ky","name":"Kyrgyz"},{"code":"lo","name":"Lao"},{"code":"la","name":"Latin"},{"code":"lv","name":"Latvian"},{"code":"lt","name":"Lithuanian"},{"code":"lb","name":"Luxembourgish"},{"code":"mk","name":"Macedonian"},{"code":"mg","name":"Malagasy"},{"code":"ms","name":"Malay"},{"code":"ml","name":"Malayalam"},{"code":"mt","name":"Maltese"},{"code":"mi","name":"Maori"},{"code":"mr","name":"Marathi"},{"code":"mn","name":"Mongolian"},{"code":"my","name":"Myanmar (Burmese)"},{"code":"ne","name":"Nepali"},{"code":"no","name":"Norwegian"},{"code":"ps","name":"Pashto"},{"code":"fa","name":"Persian"},{"code":"pl","name":"Polish"},{"code":"pt","name":"Portuguese"},{"code":"pa","name":"Punjabi"},{"code":"ro","name":"Romanian"},{"code":"ru","name":"Russian"},{"code":"sm","name":"Samoan"},{"code":"gd","name":"Scots Gaelic"},{"code":"sr","name":"Serbian"},{"code":"st","name":"Sesotho"},{"code":"sn","name":"Shona"},{"code":"sd","name":"Sindhi"},{"code":"si","name":"Sinhala"},{"code":"sk","name":"Slovak"},{"code":"sl","name":"Slovenian"},{"code":"so","name":"Somali"},{"code":"es","name":"Spanish"},{"code":"su","name":"Sundanese"},{"code":"sw","name":"Swahili"},{"code":"sv","name":"Swedish"},{"code":"tg","name":"Tajik"},{"code":"ta","name":"Tamil"},{"code":"te","name":"Telugu"},{"code":"th","name":"Thai"},{"code":"tr","name":"Turkish"},{"code":"uk","name":"Ukrainian"},{"code":"ur","name":"Urdu"},{"code":"uz","name":"Uzbek"},{"code":"vi","name":"Vietnamese"},{"code":"cy","name":"Welsh"},{"code":"xh","name":"Xhosa"},{"code":"yi","name":"Yiddish"},{"code":"yo","name":"Yoruba"},{"code":"zu","name":"Zulu"}]

```

Detect language

```
curl -X GET -H "Accept:application/json" https://merriam.io/api/v1/detect.json?t[]=hola&t[]=Bonjour&key=<your-api-key>

[{"text":"hola","results":[{"confidence":0.91015625,"language":"es"}]},{"text":"Bonjour","results":[{"confidence":0.96875,"language":"fr"}]}]
```

Translate Text


```
curl -X GET -H "Accept:application/json" https://merriam.io/api/v1/translate_text.json?t=Bonjour&c=en&key=<your-api-key>

{"text":"Hello","to":"en","origin":"Bonjour","from":"fr","model":null,"detected":true}
```

## Versioning

This library follows [Semantic Versioning](http://semver.org/).

Please note it is currently under active development. Any release versioned 0.x.y is subject to backwards incompatible changes at any time.

**GA**: Libraries defined at the GA (general availability) quality level are stable. The code surface will not change in backwards-incompatible ways unless absolutely necessary (e.g. because of critical security issues) or with an extensive deprecation period. Issues and requests against GA libraries are addressed with the highest priority.

Please note that the auto-generated portions of the GA libraries (the ones in modules such as `v1` or `v2`) are considered to be of **Beta** quality, even if the libraries that wrap them are GA.

**Beta**: Libraries defined at a Beta quality level are expected to be mostly stable and we're working towards their release candidate. We will address issues and requests with a higher priority.

**Alpha**: Libraries defined at an Alpha quality level are still a work-in-progress and are more likely to get backwards-incompatible updates.


## Contributing

Contributions to this library are always welcome and highly encouraged.

See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to get started.

## License

This library is licensed under Apache 2.0. Full license text is
available in [LICENSE](LICENSE).

## Support

Please [report bugs at the project on Github](https://github.com/MerriamIO/<library>/issues).

## Owned By

7Precision, Inc
