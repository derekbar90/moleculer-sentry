# moleculer-sentry

[![Build Status](https://travis-ci.org/YourSoftRun/moleculer-sentry.svg?branch=master)](https://travis-ci.org/YourSoftRun/moleculer-sentry)
[![Coverage Status](https://coveralls.io/repos/github/YourSoftRun/moleculer-sentry/badge.svg?branch=master)](https://coveralls.io/github/YourSoftRun/moleculer-sentry?branch=master)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/cb024436e1a84097b81775692d38ca8a)](https://www.codacy.com/app/Hugome/moleculer-sentry?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=YourSoftRun/moleculer-sentry&amp;utm_campaign=Badge_Grade)
[![Maintainability](https://api.codeclimate.com/v1/badges/166736a1d7ffb6638647/maintainability)](https://codeclimate.com/github/YourSoftRun/moleculer-sentry/maintainability)
[![David](https://img.shields.io/david/YourSoftRun/moleculer-sentry.svg)](https://david-dm.org/YourSoftRun/moleculer-sentry)
[![Known Vulnerabilities](https://snyk.io/test/github/YourSoftRun/moleculer-sentry/badge.svg)](https://snyk.io/test/github/YourSoftRun/moleculer-sentry)

[![Downloads](https://img.shields.io/npm/dm/moleculer-sentry.svg)](https://www.npmjs.com/package/moleculer-sentry)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FYourSoftRun%2Fmoleculer-sentry.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FYourSoftRun%2Fmoleculer-sentry?ref=badge_shield)

## How to use it
```js
const SentryMixin = require('moleculer-sentry')

module.exports = {
  mixins: [SentryMixin],
  settings: {
    /** @type {String} DSN given by sentry. */
    dsn: null,
    /** @type {Object?} Additional options for `Sentry.init` */
    options: {},
    /** @type {Object?} Options for the sentry scope */
    scope: {
      /** @type {String?} Name of the meta containing user infos */
      user: null
    }
  }
}
```
