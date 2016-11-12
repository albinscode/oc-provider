Open Document Provider
===

This small module allows you to open a libre office document with ODS or ODT extension.

The two embedded files `content.xml` and `footer.xml` will be available for modification.

Here is a small example:

~~~javascript
    var provider = require('od-provider');
    provider.getFromFile('myfile.odt').then(function(data) {
        console.log('Here is the content');
        console.log(data.content);
        console.log('Here is the styles content');
        console.log(data.styles);
    }
~~~
