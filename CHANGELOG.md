# CHANGELOG

## v3.1.0 (2015-07-11)
* better error messages if waitForXXX commands fail
* improved error handling
* set default logging prefs
* allow to intercept jasmine assertions
* check logging types before requesting logs
* minor bugfixes and doc improvements

## v3.0.5 (2015-07-07)
* mocha framework: allow inclusive and exclusive tests

## v3.0.4 (2015-07-07)
* fixed bug where feature files got filtered out in config parser

## v3.0.3 (2015-07-06)
* show also title of pending test (refs #606)

## v3.0.2 (2015-07-06)
* if specFn is undefined we are dealing with a pending function (fixes #606)

## v3.0.1 (2015-07-04)
* lowercase framework string (fixes #601)
* make v3 work with PhantomJS < 2.0 (fixes #594)

## v3.0.0 (2015-06-29)
* rewritten WebdriverIO core to a Monad
* removed ChainIt dependency
* implemented test runner with different reporter and support for Mocha, Jasmine and Cucumber
* added multiremote feature to control multiple instances at the same time
* enable selector chaining
* removed waitFor command (please replace it with waitForExist as it works the same way)
* new commands: [debug](http://webdriver.io/api/utility/debug.html)

## v2.4.5 (2015-01-30)
* return promise result if responseMethod is not a function (see #401)

## v2.4.4 (2015-01-24)
* make PromiseHandler to handle Q promises (see #399)

## v2.4.3 (2015-01-10)
* `saveScreenshot` doesn't require a file path anymore if only the base64 data is required (see #393)
* don't throw an error if error handler is registered (see #385)

## v2.4.2 (2015-01-07)
* fixed bug in PromiseHandler when execute command just got a single function parameter (closes #383)
* make colored logs optional (closes #298)

## v2.4.1 (2014-12-28)
* fixed bug in `selectByValue` and `selectByVisibleText` in which the absolute xPath queried value/text of different select element
* allow more xpath expressions

## v2.4.0 (2014-12-05)
* support for promises A+ (yeah!)
* introduced `waitforTimeout` option so set default timout time for all waitForXXX commands (see #345)
* let selectByValue accept number values (see #369)

## v2.3.0 (2014-10-24)
* added selectByIndex, selectByValue and selectByVisibleText for super easy selecting of options in select elements

## v2.2.3 (2014-09-18)
* support for all selector strategies in getHTML command (closes #302)

## v2.2.2 (2014-09-15)
* consider parent elements in waitForVisible command (closes #293)
* added library User-Agent string to header for statistical reporting (closes #296)
* updated examples

## v2.2.1 (2014-09-05)
* fixed bug in isVisible helper, thanks @fufnf

## v2.2.0 (2014-09-01)
* new commands:
    - [elementIdElement](http://webdriver.io/api/protocol/elementIdElement.html)
    - [elementIdElements](http://webdriver.io/api/protocol/elementIdElements.html)
    - [selectorExecute](http://webdriver.io/api/action/selectorExecute.html)
    - [selectorExecuteAsync](http://webdriver.io/api/action/selectorExecuteAsync.html)
    - [setViewportSize](http://webdriver.io/api/window/setViewportSize.html)
    - [getViewportSize](http://webdriver.io/api/window/getViewportSize.html)
* improved waitfor commands - now with support if all selector strategries (thanks to selectorExecuteAsync and @nickyout)

## v2.1.2 (2014-08-22)
* Fix: log command expecting an object and not a string
* skip close test (still to flaky)

## v2.1.1 (2014-08-20)
* took saveScreenshot functionality back to basic
* removed gm dependency since it causes too many errors when installing

## v2.1.0 (2014-08-11)
* new commands:
    - [isEnabled](http://webdriver.io/api/state/isEnabled.html)
    - [elementIdEnabled](http://webdriver.io/api/protocol/elementIdEnabled.html)
* make ErrorHandler easy accessible

## v2.0.1 (2014-08-10)
* renamed project lib constructor
* fixed isMobile detection in `chooseFile` command

## v2.0.0 (2014-08-10)
* initial release (for older releases check out the [WebdriverJS changelog](https://github.com/webdriverio/webdriverio/blob/webdriverjs/CHANGELOG.md))
