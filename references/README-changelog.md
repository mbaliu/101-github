REF: https://docs.cypress.io/guides/references/changelog


---
title: Changelog
---

## 13.6.1

_Released 12/5/2023_

**Bugfixes:**

- Fixed an issue where pages or downloads opened in a new tab were missing basic auth headers. Fixes [#28350](https://github.com/cypress-io/cypress/issues/28350).
- Fixed an issue where request logging would default the `message` to the `args` of the currently running command even though those `args` would not apply to the request log and are not displayed. If the `args` are sufficiently large (e.g. when running the `cy.task` from the [code-coverage](https://github.com/cypress-io/code-coverage/) plugin) there could be performance/memory implications. Addressed in [#28411](https://github.com/cypress-io/cypress/pull/28411).
- Fixed an issue where commands would fail with the error `must only be invoked from the spec file or support file` if the project's `baseUrl` included basic auth credentials. Fixes [#27457](https://github.com/cypress-io/cypress/issues/27457) and [#28336](https://github.com/cypress-io/cypress/issues/28336).
- Fixed an issue where some URLs would timeout in pre-request correlation. Addressed in [#28427](https://github.com/cypress-io/cypress/pull/28427).
- Cypress will now correctly log errors and debug logs on Linux machines. Fixes [#5051](https://github.com/cypress-io/cypress/issues/5051) and [#24713](https://github.com/cypress-io/cypress/issues/24713).

**Misc:**

- Artifact upload duration is now reported to Cypress Cloud. Fixes [#28238](https://github.com/cypress-io/cypress/issues/28238). Addressed in [#28418](https://github.com/cypress-io/cypress/pull/28418).
