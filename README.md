# The National Archives: Find Case Law

## Introduction

This repository is part of the [Find Case Law](https://caselaw.nationalarchives.gov.uk/) project at [The National Archives](https://www.nationalarchives.gov.uk/). For more information on the project, check [the documentation](https://github.com/nationalarchives/ds-find-caselaw-docs).

# Frontend CSS

This repository contains shared SASS and JS for the Find Case Law service. It's used across the [Editor UI](https://github.com/nationalarchives/ds-caselaw-editor-ui) and the [Public UI](https://github.com/nationalarchives/ds-caselaw-public-ui).

## Usage

This repository is _not_ listed on npm, and you will need to add the full git repository path to your `package.json`:

```json
"dependencies": {
  "@nationalarchives/ds-caselaw-frontend": "git://github.com/nationalarchives/ds-caselaw-frontend#v1.1.0",
  "sass": "^1.58.3"
}
```

Once installed, import from the correct location in your SCSS, checking that relative paths are correct:

```scss
@import "../../node_modules/@nationalarchives/ds-caselaw-frontend/src/main";
```

## Development

Check out this repo, as well as the [Editor UI](https://github.com/nationalarchives/ds-caselaw-editor-ui) and/or [Public UI](https://github.com/nationalarchives/ds-caselaw-public-ui)

In the Editor UI and/or Public UI repository run:

```console
npm link path/to/this/repo
```

to ensure your development copy loads the local version of this package.

When you're ready, create a PR on this repository. Once it is merged into main,
run `npm update` in the two applications to pull the latest `main`, and create PRs for the changes to `package-lock.json`. Once they are merged and deployed, the latest changes will be used.

## Releasing

- Update the version number in `package.json`
- Tag the new release in GitHub
