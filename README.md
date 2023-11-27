# Motivation

This repo is a perfect solution when you need to develop a new website that only contains the HTML and CSS files. For example, a theme for WordPress or any other CMS that requires you only the html/css files, or you just wanna learn the [SASS](https://sass-lang.com/) in isulation.

## Requirements

- [Node](https://nodejs.org/en/) `^16.15.0`
- [NPM](https://www.npmjs.com/) `^8.5.5`

## Installation

After confirming that your environment meets the
above [requirements](#requirements), it is time to clone the project
locally by doing the following:

```bash
$ git clone https://github.com/DeanHristov/html-scss-starter-kit.git <project-name>
$ cd <project-name>
```

When you're done with the steps above, run the following command:

```bash
$ npm install # or yarn install
```

## Project Structure

```
├── dist                # Contains **production-ready** code. Put any other types of files here.
│   └── index.html      # The entry page of the site
│   └── *.html          # Sub-pages
│   └── css             # Contains all compiled styles
│       └── main.css    # the Main style. It is used from the index.html
│       └── *.css       # Other styles belong to sub-pages
├── scss                # Contains all SCSS based styles (variables, mixins ....) splitted by modules
│   └── *.scss          # Other styles like (variables, mixins ....)
│   └── main.css        # The entry point of the styles
├── package.json        # It holds important metadata about a project like scripts dependencies
├── package-lock.json   # Place where we controls the dependencies
├── README.md           # A documentation file
```

## Main tasks

All tasks automation are based on [NPM scripts](https://docs.npmjs.com/misc/scripts).

| Tasks               | Description                                      |
| ------------------- | ------------------------------------------------ |
| `npm run watch`     | Watching the styles fro changes                  |
| `npm run build`     | Building the styles in **production-ready** code |
| `npm run start:dev` | Running the the page in **dev** mode with HMR    |

## Running the

Running the page in **development** mode.

```bash
$ npm run start:dev
```

## Running the page in production mode.

Compiling the styles in production-ready mode within **~/dist** directory.

```bash
$ npm run build
```

## Used technologies

- NodeJS - https://nodejs.org/en/
- Git - https://git-scm.com/
- SCSS - https://sass-lang.com/

## NPM Packages

- [concurrently](https://www.npmjs.com/package/concurrently)
- [live-server](https://www.npmjs.com/package/live-server)
- [node-sass](https://www.npmjs.com/package/node-sass)

## Made by

Author: [D. Hristov](https://dhristov.eu/)
