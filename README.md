# weifund-lib

[![NPM version](http://img.shields.io/npm/v/weifund-lib.svg)](https://www.npmjs.org/package/weifund-lib) [![Build status](https://ci.appveyor.com/api/projects/status/wwajr0886e00g8je/branch/master?svg=true)](https://ci.appveyor.com/project/weifund/weifund-lib/branch/master) [![Coverage Status](https://coveralls.io/repos/github/weifund/weifund-lib/badge.svg?branch=master)](https://coveralls.io/github/weifund/weifund-lib?branch=master) [![NPM Downloads](https://img.shields.io/npm/dm/weifund-lib.svg)](https://www.npmjs.org/package/weifund-lib)

A library with all WeiFund campaign data retrieval methods.

## Install

```
npm install
```

## Future Design/Usage

```js
// get campaigns method
const getCampaigns = require('weifund-lib').getCampaigns;

// get campaigns
getCampaigns({
  // set network
  // or 'testnet'
  network: 'testnet',

  // set campaign selector
  // array (i.e. array of campaignIDs)
  selector: [0],

  // set web3 provider
  web3Provider: {},

  // set ipfs provider
  ipfsProvider: {},
}, function (getCampaignError, campaignsResult) {
  // async callback with either error or camapign result
  console.log(campaignsResult);
});
```

## About

The WeiFund library. This contains all methods needed to pull campaign data from IPFS or the blockchain.

## Contributing

Please help better the ecosystem by submitting issues and pull requests to weifund-lib. We need all the help we can get to build the absolute best linting standards and utilities. We follow the AirBNB linting standard. Please read more about contributing to `weifund-lib` in the `CONTRIBUTING.md`.

## Guides

You'll find more detailed information on using weifund-lib and tailoring it to your needs in our guides:

- [User guide](docs/user-guide.md) - Usage, configuration, FAQ and complementary tools.
- [Developer guide](docs/developer-guide.md) - Contributing to weifund-lib and writing your own plugins & formatters.

## Help out

There is always a lot of work to do, and will have many rules to maintain. So please help out in any way that you can:

- Create, enhance, and debug rules (see our guide to ["Working on rules"](CONTRIBUTING.md)).
- Improve documentation.
- Chime in on any open issue or pull request.
- Open new issues about your ideas for making stylelint better, and pull requests to show us how your idea works.
- Add new tests to *absolutely anything*.
- Work on [improving performance of rules](docs/developer-guide/benchmarks.md).
- Create or contribute to ecosystem tools, like the plugins for Atom and Sublime Text.
- Spread the word.

Please consult our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing](CONTRIBUTING.md) docs before helping out.

We communicate via [issues](https://github.com/weifund/weifund-lib/issues) and [pull requests](https://github.com/weifund/weifund-lib/pulls).

## Important documents

- [Changelog](CHANGELOG.md)
- [Contributing Guidelines](CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](https://raw.githubusercontent.com/weifund/weifund-lib/master/LICENSE)

## Licence

```
The MIT License

Copyright (c) 2016 WeiFund. www.weifund.io

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
