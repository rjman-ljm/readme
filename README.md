<p align="center">
  <img src="https://avatars1.githubusercontent.com/u/6267397?s=460&v=4" alt="Logo" width="100" height="auto" />
</p>

<h1 align="center">@appnest/readme</h1>
<p align="center">
		<a href="https://npmcharts.com/compare/{{ readme.ids.npm }}?minimal=true"><img alt="Downloads per month" src="https://img.shields.io/npm/dm/{{ readme.ids.npm }}.svg" height="20"/></a>
<a href="https://www.npmjs.com/package/{{ readme.ids.npm }}"><img alt="NPM Version" src="https://img.shields.io/npm/v/{{ readme.ids.npm }}.svg" height="20"/></a>
<a href="https://david-dm.org/{{ readme.ids.github }}"><img alt="Dependencies" src="https://img.shields.io/david/{{ readme.ids.github }}.svg" height="20"/></a>
<a href="https://github.com/{{ readme.ids.github }}/graphs/contributors"><img alt="Contributors" src="https://img.shields.io/github/contributors/{{ readme.ids.github }}.svg" height="20"/></a>
	</p>
<p align="center">
  <b>Generate pretty README.md files with your new superpowers!</b></br>
  <sub>Use this readme generator to easily generate pretty readme's like this one! Simply extend your <code>package.json</code> and create a readme blueprint.<sub>
</p>

<br />

* Bullet 1
* Bullet 2
* Bullet 3

<p>IMAGE</p>

## Table of Contents

* [❯ 1. Installation](#-1-installation)
* [❯ 2. Create a blueprint](#-2-create-a-blueprint)
* [❯ Contributors](#-contributors)
* [❯ License](#-license)

![line](https://github.com/andreasbm/readme/blob/master/assets/line.png)

## ❯ 1. Installation

```javascript
npm install @appnest/readme
```
![line](https://github.com/andreasbm/readme/blob/master/assets/line.png)

## ❯ 2. Create a blueprint

First you need to create a `blueprint.md` file (name it whatever you like). This blueprint is going to be the blueprint for the `README.md` file we are going to generate later.

Let's start simple. In order to get values from your `package.json` file injected into the readme we use the `{{ .. }}` syntax. Let's say your `package.json` file looks like this:

```json
{
  "name": "@appnest/readme",
  "version": "1.0.0"
}
```

To get the `name` and `version` into your readme you will need to write `{{ name }}` and `{{ version }}` in your `blueprint.md` file like this:

```markdown
Welcome to {{ name }}. This is version {{ version }}!
```

When running `node node_modules/.bin/readme --input=blueprint.md --output=README.md` the file `README.md` will be generated with the following contents:

```markdown
Welcome to @appnest/readme. This is version 1.0.0.
```



![line](https://github.com/andreasbm/readme/blob/master/assets/line.png)

## ❯ Contributors
	
* <a href="https://twitter.com/andreasmehlsen">Andreas Mehlsen</a> (<a href="mailto:andmehlsen@gmail.com">andmehlsen@gmail.com</a>)

![line](https://github.com/andreasbm/readme/blob/master/assets/line.png)

## ❯ License
	
Licensed under [MIT](https://opensource.org/licenses/MIT).