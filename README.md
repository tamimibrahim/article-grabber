# article-grabber

> A Node.js module to retrieve article content and metadata from a URL.


## Extracting data
```js
var extractor = require('article-grabber');

extractor.extractData('http://somesite.com/apage.html', function (err, data) {
  console.log(data);
});

```

## Extract result
The result looks like this:
```json
{
    "domain": "somesite.com",
    "author": "Jhone doe",
    "title": "An article title",
    "summary": "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Qui, maxime?",
    "content": "<h1>Lorem ipsum dolor sit.</h1><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore, possimus.</p><h2>Lorem ipsum dolor sit amet.</h2><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. <img src="image.png" alt=""> Pariatur dolor deleniti esse repellendus accusamus ducimus aut molestias optio obcaecati similique.</p>"
}
```
