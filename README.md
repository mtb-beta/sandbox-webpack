# sandbox-webpack
Sandbox for Webpack

# sample1

install webpack, and build simple script.

first, init npm.

```
npm init -y
```

install webpack, and webpack-cli.

```
npm install -D webpack webpack-cli
```

create src/index.js as below.

```
$ cat src/index.js
let message = "hello webpack";

console.log(message);
```

check index.js.

```
$ node src/index.js
hello webpack
```

add build command on npm run.
update script objects as below in package.json.

```
  "scripts": {
    "build": "webpack"
  },
```

build index.js by webpack by next command.
```
$ npm run build
```

check main.js, which is a post-build index.js.

```
$ node dist/main.js
hello webpack
```

