# referee

[![Build status](https://secure.travis-ci.org/busterjs/referee.png?branch=master)](http://travis-ci.org/busterjs/referee)

**referee** is in your unit tests, deciding who passes and who fails.

It is a test-framework agnostic assertion and expectation library.
Some highlights:

- Rich library of assertions
- Symmetric assert/refute (refute is **referee**'s "assert.not*")
- Evented: Emits success and failure events
- Failing assertions throw exceptions by default, but can be configured to not
- API to add custom assertions that provides quite a bit of plumbing for free

Full documentation:
[docs.busterjs.org/en/latest/modules/referee](http://docs.busterjs.org/en/latest/modules/referee/).

**referee** works in browsers (including old and rowdy ones, like IE6) and Node.
It will define itself as an AMD module if you want it to (i.e. if there's a
`define` function available).

## Developers - Running tests

### Node

  1. `npm install` - installs dev dependencies
  1. `npm test` - runs node tests
    
### Browsers

  1. `npm install` - installs dev dependencies
  1. `npm start` - starts buster server
  1. open url localhost:1111/capture in the browser(s) you want to test with
  1. `npm run-script test-browser` - runs browser tests