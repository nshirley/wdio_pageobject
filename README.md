# WIP

### Getting started

bare bones project for wrapping up page objects. The use here is to pull them into various projects that need them rather than each project having their own implementation.
This project is _only_ written with typescript as webdriverio (as of V7) supports JIT transpile of typescript to js, eliminating the need for running tsc and packaging builds.

### Requirements

For consumption

- webdriverio: >= 7.0

Follow the setup steps here `<INSERT_LINK>` on how to get started with a new webdriverio project that leverages typescript natively. Alternatively, you can use the template project here `<INSERT_LINK>`

---

## Usage

Since this package is built on _only_ Typescript, your consumption must leverage that with webdriverio, an example on setup can be found [here](https://webdriver.io/docs/typescript/).

#### Installation

```
$> yarn add @SOME_REPO/wdio_pageobjects
```

#### Implementation

All PageObjects are exposed by a CamelCased instance appended with `Page` ie. `StudentHomePage`. To access them a simple import is needed as such `import { StudentHomePage } from "@SOME_REPO/wdio_pageobjects"`

---

### Local development

If you're contributing to this project and want to test your page.objects before pushing, you can use `yarn link` to create a symlink locally of the packaged then -> `yarn link <packaged_name>` to use it in another project locally

### Publish

TBD

### Contribution

Please make sure test page.objects locally before publishing. ONLY `main` should be published from, this helps require a review of your changes before publishing.
