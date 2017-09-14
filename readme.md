# Cypress CLI [![Circle CI](https://circleci.com/gh/cypress-io/cypress-cli.svg?style=shield)](https://circleci.com/gh/cypress-io/cypress-cli)

This is the CLI for: [https://github.com/cypress-io/cypress](https://github.com/cypress-io/cypress).

## Deprecated

⚠️ This module is deprecated in favor of an "all-in-one" Cypress NPM package
`cypress` that can be installed as a regular dev dependency.

See [https://on.cypress.io/installing-via-npm](https://on.cypress.io/installing-via-npm)

## Installing new versions

This module is now limited to installing older versions of Cypress.
When trying to install a "new" version of Cypress module (>= 0.20.0) CLI will exit with an
error. Similarly, if you do not specify the explicit old version, it will not allow installing the latest Cypress version

```text
$ cypress-cli install
You are trying to install the latest version of Cypress.

This CLI tool is deprecated and can no longer install versions of Cypress above 0.19.4.

For newer versions, please use the new cypress npm module.

See https://on.cypress.io/installing-cypress for details
```

## Documentation

[The documentation has moved into our official docs here.](https://on.cypress.io/cli)

## Changelog

#### 0.13.1 - *(02/11/17)*
- add --record option, pass --cli-version to cypress

#### 0.13.0 - *(02/11/17)*
- deprecated 'cypress ci'
- 'cypress run' now accepts a --key argument and a --record false argument
- search for CYPRESS_RECORD_KEY env var
- more intelligently spawn XVFB
- some horrid code cleanup

#### 0.12.2 - *(01/21/17)*
- bump core releaser

#### 0.12.1
- bump update-notifier dep for configstore fixes

#### 0.12.0
- added cli arg for passing reporterOptions

#### 0.11.1
- cypress ci accepts --spec argument

#### 0.11.0
- `cypress open` now accepts arguments
- you can now pass the --config flag to `cypress run`, `ci`, and `open` which overrides `cypress.json` configuration values
