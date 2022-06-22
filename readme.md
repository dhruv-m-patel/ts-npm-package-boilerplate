# ts-npm-package-boilerplate

A boilerplate to build npm package with typescript

### Using this boilerplate package repo

1. Get the boilerplate:
   - This repo is marked as a template, so you can use it to create your own package directly from github.
   - You can clone this repo using `git clone git@github.com:dhruv-m-patel/ts-npm-package-boilerplate.git`

2. On your github repo, go to Settings > Security / Secrets, and add a Repository Secret with name `NPM_TOKEN` and add your npm token as value with write access to your npm registry.

### Features

- Minimal boilerplate with typescript, eslint, husky hooks and prettier integration to enforce best practices
- `.npmignore` added to ignore unnecessary resources getting published and keeping published package size lower
- By default integrated with Github Actions for CI/CD
- Auto-publishes package to your npm registry whenever tags are pushed to Github repository.

**Note:** If you are planning to use this boilerplate for a `private` package, you MUST edit `.github/workflows/publish.yml` and drop `--access public` on line #32.
