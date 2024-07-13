## Setting up the Server

Create a folder for the server and create a file index.js in it. Also create an .env file to store the environment variables.

```bash
NODE_ENV='development'
PORT=5001

```

Initialize and start the server:

```js
const express = require("express");
const app = express();
require("dotenv").config();
const port = process.env.PORT || 6000;

app.listen(port, console.log(`App listening on port : ${port}`));
```
