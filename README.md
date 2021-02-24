# TypeScript in Node.js

This is a boiler plate for typescript and node.js

## Usage

> To use this boiler plate clone this repository by running the following command

```shell
$ git clone https://github.com/
```

> Navigate to the boiler-plate folder by running the following command

```shell
$ cd tsnode-boiler-plate
```

> Install all dependencies by running the following command

```shell
$ npm install
```

> Then

```shell
$ npm start
```

### Setup

#### Step 1: Create a `package.js` file

To create a `package.json` file run the following command:

```shell
$ npm init -y
```

> To create a `package.json` file with default options

#### Step 2: Install all the dependencies

To use typescript install the following dependencies by running the following command:

```shell
$ npm install -save-dev typescript
$ npm install -save-dev tslint
$ npm install express -save
$ npm install @types/express -save-dev
```

#### Step 3: Create a `tsconfig.json` file in the root directory.

To create a `tsconfig.json` file run the following command:

```
$ touch tsconfig.json
```

> Alternatively you can create it manually. Open the file and add the following code in it

```
{
    "compilerOptions": {
      "module": "commonjs",
      "esModuleInterop": true,
      "target": "es6",
      "moduleResolution": "node",
      "sourceMap": true,
      "outDir": "dist"
    },
    "lib": ["es2015"]
}
```

#### Step 4: Create a `tslint.json` file in the root directory.

To create a `tslint.json` file run the following command:

```
$ touch tslint.json
```

> Alternatively you can create it manually. Open the file and add the following code in it

```
{
    "defaultSeverity": "error",
    "extends": [
        "tslint:recommended"
    ],
    "jsRules": {},
    "rules": {
        "no-console":false
    },
    "rulesDirectory": []
}
```

#### Step 5: Modify your `package.json` file to look as follows:

```
{
  "name": "tsnode-boiler-plate",
  "version": "1.0.0",
  "description": "",
  "main": "dist/app.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "tsc && node dist/app.js"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "@types/express": "^4.17.11",
    "tslint": "^6.1.3",
    "typescript": "^4.2.2"
  },
  "dependencies": {
    "express": "^4.17.1"
  }
}

```

#### Step 6: Create a app.ts file in the src directory

Populate it with the following code:

```
const message: string = "Hello world!\n Go to the src/app.ts and start coding";

console.log(message);

```

Then run the following command:

```shell
$ npm start
```

That's all you need

### Credits

- None
