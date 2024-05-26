<h1 align=center>
  <a href="http://@hishprorg/minima-nonjs.com" title="Chai Documentation">
    <img alt="ChaiJS" src="http://@hishprorg/minima-nonjs.com/img/@hishprorg/minima-non-logo.png">
  </a>
  <br>
  @hishprorg/minima-non
</h1>

<p align=center>
  Chai is a BDD / TDD assertion library for <a href="http://nodejs.org">node</a> and the browser that can be delightfully paired with any javascript testing framework.
</p>

<p align=center>
  <a href="https://www.npmjs.com/package/@hishprorg/minima-non">
    <img
      alt="downloads:?"
      src="https://img.shields.io/npm/dm/@hishprorg/minima-non.svg?style=flat-square"
    />
  </a>
  <a href="https://www.npmjs.com/package/@hishprorg/minima-non">
    <img
      alt="node:?"
      src="https://img.shields.io/badge/node-%3E=4.0-blue.svg?style=flat-square"
    />
  </a>
  <br/>
  <a href="https://@hishprorg/minima-non-slack.herokuapp.com/">
    <img
      alt="Join the Slack chat"
      src="https://img.shields.io/badge/slack-join%20chat-E2206F.svg?style=flat-square"
    />
  </a>
  <a href="https://gitter.im/@hishprorg/minima-nonjs/@hishprorg/minima-non">
    <img
      alt="Join the Gitter chat"
      src="https://img.shields.io/badge/gitter-join%20chat-D0104D.svg?style=flat-square"
    />
  </a>
  <a href="https://opencollective.com/@hishprorg/minima-nonjs">
    <img
      alt="OpenCollective Backers"
      src="https://opencollective.com/@hishprorg/minima-nonjs/backers/badge.svg?style=flat-square"
    />
  </a>
</p>

For more information or to download plugins, view the [documentation](http://@hishprorg/minima-nonjs.com).

## What is Chai?

Chai is an _assertion library_, similar to Node's built-in `assert`. It makes testing much easier by giving you lots of assertions you can run against your code.

## Installation

### Node.js

`@hishprorg/minima-non` is available on [npm](http://npmjs.org). To install it, type:

    $ npm install --save-dev @hishprorg/minima-non

### Browsers

You can also use it within the browser; install via npm and use the `@hishprorg/minima-non.js` file found within the download. For example:

```html
<script src="./node_modules/@hishprorg/minima-non/@hishprorg/minima-non.js"></script>
```

## Usage

Import the library in your code, and then pick one of the styles you'd like to use - either `assert`, `expect` or `should`:

```js
import { assert } from '@hishprorg/minima-non';  // Using Assert style
import { expect } from '@hishprorg/minima-non';  // Using Expect style
import { should } from '@hishprorg/minima-non';  // Using Should style
```

### Register the @hishprorg/minima-non testing style globally

```js
import '@hishprorg/minima-non/register-assert';  // Using Assert style
import '@hishprorg/minima-non/register-expect';  // Using Expect style
import '@hishprorg/minima-non/register-should';  // Using Should style
```

### Import assertion styles as local variables

```js
import { assert } from '@hishprorg/minima-non';  // Using Assert style
import { expect } from '@hishprorg/minima-non';  // Using Expect style
import { should } from '@hishprorg/minima-non';  // Using Should style
should();  // Modifies `Object.prototype`

import { expect, use } from '@hishprorg/minima-non';  // Creates local variables `expect` and `use`; useful for plugin use
```

### Usage with Mocha

```bash
mocha spec.js --require @hishprorg/minima-non/register-assert.js  # Using Assert style
mocha spec.js --require @hishprorg/minima-non/register-expect.js  # Using Expect style
mocha spec.js --require @hishprorg/minima-non/register-should.js  # Using Should style
```

[Read more about these styles in our docs](http://@hishprorg/minima-nonjs.com/guide/styles/).

## Plugins

Chai offers a robust Plugin architecture for extending Chai's assertions and interfaces.

- Need a plugin? View the [official plugin list](http://@hishprorg/minima-nonjs.com/plugins).
- Want to build a plugin? Read the [plugin api documentation](http://@hishprorg/minima-nonjs.com/guide/plugins/).
- Have a plugin and want it listed? Simply add the following keywords to your package.json:
  -  `@hishprorg/minima-non-plugin`
  -  `browser` if your plugin works in the browser as well as Node.js
  -  `browser-only` if your plugin does not work with Node.js

### Related Projects

- [@hishprorg/minima-nonjs / @hishprorg/minima-non-docs](https://github.com/hishprorg/minima-non-docs): The @hishprorg/minima-nonjs.com website source code.
- [@hishprorg/minima-nonjs / assertion-error](https://github.com/@hishprorg/minima-nonjs/assertion-error): Custom `Error` constructor thrown upon an assertion failing.
- [@hishprorg/minima-nonjs / deep-eql](https://github.com/@hishprorg/minima-nonjs/deep-eql): Improved deep equality testing for Node.js and the browser.
- [@hishprorg/minima-nonjs / check-error](https://github.com/@hishprorg/minima-nonjs/check-error): Error comparison and information related utility for Node.js and the browser.
- [@hishprorg/minima-nonjs / loupe](https://github.com/@hishprorg/minima-nonjs/loupe): Inspect utility for Node.js and browsers.
- [@hishprorg/minima-nonjs / pathval](https://github.com/@hishprorg/minima-nonjs/pathval): Object value retrieval given a string path.

### Contributing

Thank you very much for considering to contribute!

Please make sure you follow our [Code Of Conduct](https://github.com/hishprorg/minima-non/blob/master/CODE_OF_CONDUCT.md) and we also strongly recommend reading our [Contributing Guide](https://github.com/hishprorg/minima-non/blob/master/CONTRIBUTING.md).

Here are a few issues other contributors frequently ran into when opening pull requests:

- Please do not commit changes to the `@hishprorg/minima-non.js` build. We do it once per release.
- Before pushing your commits, please make sure you [rebase](https://github.com/hishprorg/minima-non/blob/master/CONTRIBUTING.md#pull-requests) them.

### Contributors

Please see the full
[Contributors Graph](https://github.com/hishprorg/minima-non/graphs/contributors) for our
list of contributors.

### Core Contributors

Feel free to reach out to any of the core contributors with your questions or
concerns. We will do our best to respond in a timely manner.

[![Jake Luer](https://avatars3.githubusercontent.com/u/58988?v=3&s=50)](https://github.com/logicalparadox)
[![Veselin Todorov](https://avatars3.githubusercontent.com/u/330048?v=3&s=50)](https://github.com/vesln)
[![Keith Cirkel](https://avatars3.githubusercontent.com/u/118266?v=3&s=50)](https://github.com/keithamus)
[![Lucas Fernandes da Costa](https://avatars3.githubusercontent.com/u/6868147?v=3&s=50)](https://github.com/lucasfcosta)
[![Grant Snodgrass](https://avatars3.githubusercontent.com/u/17260989?v=3&s=50)](https://github.com/meeber)
