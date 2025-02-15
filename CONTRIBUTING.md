<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

**Table of Contents** _generated with [DocToc](https://github.com/thlorenz/doctoc)_

- [Contributing guidelines](#contributing-guidelines)
  - [Commit sign-off](#commit-sign-off)
  - [Contributions](#contributions)
  - [Certificate of Origin](#certificate-of-origin)
  - [Contributing A Patch](#contributing-a-patch)
  - [Issue and Pull Request Management](#issue-and-pull-request-management)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Commit sign-off

To commit your changes, you would need to sign off on your commit:

```
git commit -s -m ....
```

To amend a previous commit:

```
git commit --amend --signoff
```

You can also mass sign-off a whole pull request with

```
git rebase --signoff ${BASE_BRANCH_NAME}
```

# Contributing guidelines

## Contributions

All contributions to the repository must be submitted under the terms of the [Apache Public License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

## Certificate of Origin

By contributing to this project you agree to the Developer Certificate of
Origin (DCO). This document was created by the Linux Kernel community and is a
simple statement that you, as a contributor, have the legal right to make the
contribution. See the [DCO](DCO) file for details.

## Contributing A Patch

1. Submit an issue describing your proposed change to the repo in question.
1. The [repo owners](OWNERS) will respond to your issue promptly.
1. Fork the desired repo, develop and test your code changes.
1. Submit a pull request.

## Issue and Pull Request Management

Anyone may comment on issues and submit reviews for pull requests. However, in
order to be assigned an issue or pull request, you must be a member of the
[stolostron](https://github.com/stolostron) GitHub organization.

Repo maintainers can assign you an issue or pull request by leaving a
`/assign <your Github ID>` comment on the issue or pull request.

Now, you can follow the [getting started guide](./README.md#getting-started) to work with the stolostron application-chart repository.
