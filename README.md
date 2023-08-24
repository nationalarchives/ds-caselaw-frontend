# DS Caselaw Frontend
## Introduction

This repository contains shared SASS and JS for the [Find caselaw service](https://caselaw.nationalarchives.gov.uk/), it's used across the Editor UI[Editor UI](https://github.com/nationalarchives/ds-caselaw-editor-ui) and the [Public UI](https://github.com/nationalarchives/ds-caselaw-public-ui).

## Contents

- The SASS for displaying judgment text, in `src/includes/_judgment_text.scss`

## Development

Check out this repo, as well as the [Editor UI](https://github.com/nationalarchives/ds-caselaw-editor-ui) and/or [Public UI](https://github.com/nationalarchives/ds-caselaw-public-ui)

In the Editor UI and/or Public UI repository run:

```console
npm link path/to/this/repo
```

to ensure your development copy loads the local version of this package.

When you're ready, create a PR on this repository. Once it is merged into main,
run `npm update` in the two applications to pull the latest `main`, and create PRs for the changes to `package-lock.json`. Once they are merged and deployed, the latest changes will be used.
