---
title: How to contribute
icon: true

---

Contributions to WhitestormJS are welcome; to make things easier, we've included a [Getting Started](https://github.com/WhitestormJS/whitestorm.js/blob/beta/.github/CONTRIBUTING.md#getting-started) section.

We look forward to your contributions to WhitestormJS.

![](http://i.imgur.com/Mh5HMEn.png)

## Getting Started

### Reporting Bugs

If you've found a *reproduceable* bug, [submit an issue](https://github.com/WhitestormJS/whitestorm.js/issues)! If you're sure that the issue is caused by WhitestormJS, submitting an issue will help us fix the problem.

**Don't forget to check "bug" in issue type**
```
 - [x] Bug
 - [ ] Proposal/Enhancement
 - [ ] Question
 - [ ] Discussion
```

You're welcome to fix things for us, and submit pull requests; it frees up time for us to implement useful new features.

### Adding Features

If you've added a new feature to WhitestormJS and would like for it to be included, submit a pull request. We'll take a look at it.

### Want to help us? Take a task!

We have a [task board](https://github.com/WhitestormJS/whitestorm.js/projects/4) where we keep all TODOs sorted by it's priority.

[![](http://i.imgur.com/KYmYwN7.png)](https://github.com/WhitestormJS/whitestorm.js/projects/4)

Before starting contributing it's better to contact us in [discord](https://discordapp.com/invite/frNetGE):
 - [@sasha240100](https://github.com/sasha240100) (`@alex2401#9076` in discord)
 - [@hirako2000](https://github.com/hirako2000) (`@Hirako#4563` in discord)
 - [@thejmazz](https://github.com/thejmazz) (`@thejmazz#3954` in discord)

### How to make a PR (Pull Request)

1. First of all you should **check if there is an issue that you will fix with your PR**.
2. Then you should go and **make a new branch** with name `#xxx` (Issue number)
3. **Make changes**
4. **Submit a PR!**
   - If PR is related to an issue - 📌 **refer to that issue in PR description**.

### Building WhitestormJS

WhitestormJS can be built by installing [Node.js](https://nodejs.org), and the [gulp](https://www.npmjs.com/package/gulp) package through [npm](https://www.npmjs.com/).

After that, clone the repository anywhere you'd like (`git clone https://github.com/WhitestormJS/whitestorm.js.git`).

Open the new directory (`./WhitestormJS/` by default) using whatever terminal emulator you'd like.

You can build WhitestormJS with the following command: `npm run build`

WhitestormJS will be built, and written to `build/whitestorm.js`, and `build/whitestorm.compact.js`.

```bash
$ git clone https://github.com/WhitestormJS/whitestorm.js.git
$ cd whitestorm.js
$ npm install
$ npm run build
```

### CLI

#### Development mode
`npm start`
- Starts `webpack-dev-server` for whs sources.
- Starts `webpack-dev-server` for each example located in `./examples`
- Starts `gulp less:watch`
  - Watches each `.less` in `./examples/assets/less`
  - Compiles to `./examples/assets/css`

![](http://i.imgur.com/7bDhpHK.png)

#### Build all
`npm run build`
- Runs `gulp build` - build sources
- Runs `gulp examples:build` - build examples

![](http://i.imgur.com/AfIQY8l.png)

#### Unit testing, coverage, snyk
`npm test`
Runs all testing suites. Used in Travis CI for this project.

![](http://i.imgur.com/WbWMykP.png)

#### Deploy examples
`npm run deploy`
> Only for those, **who are in dev team and have write access on surge.sh for examples domain**

----

### Committing

All engine code is in the `src/` folder.
Modules are in the `modules/`, each having their own build.

_We still in the process of moving all remaining modules from `src/` to `modules`. If you create a new module, please put it in the `modules` folder._

**Do not edit files in `build/` folder!!!*

### Commit messages

#### Codes
 - **CSF** - Code style fix. (Comes with file name.)
 - **TU** - Temporary update. (Will be changed later.)
 - **README** - You changed README.md file.
 - **LICENSE** - You changed LICENSE.md file.
 - **CONTRIBUTING.** - You changed CONTRIBUTING.md file.



#### Fixed Issue

If your commit fixes for an _issue_ on github, you must add `Fixed #25`. Where **#25 is ID of the issue.**

#### Syntax

- **Code** - e.g `CSF.` or `TU.` (If your commit matches one of them.)
- **Comment** - Your comment to commit. (optional, unless you have no code.)
- **Fix** - Example: `Fixed #25`. (If you fixed issue #25)

>**code must be UPPCERCASE, comment must be be Capitalized**

>**If you have `CSF` your comment must be the name of the file you fixed.** No dot after filename


#### Examples

Good:
 - `CSF: ShaderTerrain.js Fixed #25`
 - `Edited core module`

Poor:
 - `Changes..`
 - `Fixed #25`
 - `Fixed code style.` (Use "CSF")
 - `WIPSHADEERTERRAINJSFIXES####2017!!!!`


### Code style guidelines
 - Follow code style guides:
    - [XO](https://github.com/sindresorhus/xo)
    - Wrap logical blocks* with newlines.

_logical blocks_* - lines that have something in common.
