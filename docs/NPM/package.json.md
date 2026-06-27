# package.json file

This is the project main dependency file, it tells [NPM](./index.md) the configuration of your project.

## Creating the file

To create the file, you need to run this command,

```bash
npm init
```

if you want all the default settings without the CLI asking you each field, you may run one of the following,

```bash
npm init -y
npm init --yes
```

## Contents

This file contains all the configuration for the project, and the default file looks like,

```json
{
	"name": "fullstack",
	"version": "1.0.0",
	"description": "",
	"main": "index.js",
	"scripts": {
		"test": "echo \"Error: no test specified\" && exit 1"
	},
	"author": "",
	"license": "ISC",
	"type": "commonjs"
}
```

### npm scripts

The only field that isn't self explanatory is `scripts`, this field is used to run bash commands, if we run,

```bash
npm run <script-name>
```

it will run the command in the file.

For example, if we have,

```json
"scripts": {
	"hello": "echo \"World!\""
}
```

then,

```bash
>>> npm run hello
World!
```

## Changing the default

To change the default fields used by NPM, you need to use one of the following commands,

```bash
npm config set init-<field> "<new-default>"
npm set init-<field> "<new-default>"
```

for example,

```bash
npm config set init-author-name "John Doe"
npm set init-licence "MIT"
```

To get the default value,

```bash
npm config get init-<field>
npm get init-<field>
```

And to revert the default value,

```bash
npm config delete init-<field>
npm delete init-<field>
```
