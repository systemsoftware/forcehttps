# Force HTTPS
Simple Express middleware to force HTTPS.


```js
const forceHTTPS = require('forcehttps');
const express = require('express');
const app = express();

app.use(forceHTTPS);

app.get('/', (req, res) => {
  res.send('Hello World!');
});

app.listen(3000);
```