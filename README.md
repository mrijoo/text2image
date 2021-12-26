# Text2image

## Instalation :
```
npm i @mrijoo/text2image
```

## Usage:
```js
const text2image = require('@mrijoo/text2image')
```

## Example
```js
const fs = require("fs")
const text2image = require('@mrijoo/text2image');

text2image.convert('Hello, World!', "ObelixProBIt-cyr", { family: 'pg' }, { x: 70, y: 50, width: 400,  height: 400 }, {}).then(base64 => {
    fs.writeFile("out.png", base64.replace(/^data:image\/png;base64,/, ""), 'base64', function() {});
})

```