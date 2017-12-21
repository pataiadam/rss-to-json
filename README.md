

Util for parse ATOM and RSS feed resources and normalize them to JSON object.

## Install

```js
npm install pataiadam/rss-to-json --save
```

## Example

```js

var Feed = require('rss-to-json');

Feed.load('https://codek.tv/feed/')
  .then(console.log);

```
## Result
```js

  {
    "items":[
      {
        "title":"New Raspberry Pi Camera V2 Overview and Comparison",
        "description":"",
        "link":"http://codek.tv/v/rkoyPMJ-",
        "url":"http://codek.tv/v/rkoyPMJ-",
        "created":1461819107000,
        "enclosures":[
          {
            "url":"http://i.viralr.net/media/2016/03/30/3b314f65ed8f0def36825d3d1ab6561b.png",
            "length":"0",
            "type":"image/jpeg"
          }
        ]
      },
     // ...
    ],
    "title":"Ultimate Training Academy Free for Developers",
    "description":"Ultimate Free Courses, Tutorials: Node js, Angular js, Javascript, Python, Php, Wordpress, Mongodb, Nosql, C#, Ember js, React js",
    "url":"http://codek.tv"
  }
```
