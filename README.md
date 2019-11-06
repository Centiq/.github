# GitHub Templates

This repo contains Centiq-wide templates for GitHub functionality - primarily issue and pull request templates.

In order to function, this repo has to be publicly available (Internet-facing), so consider carefully before pushing anything to the repo and raising/commenting on issues/PRs.

## Usage

If a Centiq repo, whether public or private, does not have its own templates files, then these will be used as default.

The default templates are:
- [`ISSUE_TEMPLATE.md`](ISSUE_TEMPLATE.md)
- [`PULL_REQUEST_TEMPLATE.md`](PULL_REQUEST_TEMPLATE.md)

More specific templates can be selected with a little URL manipulation:
- [`ISSUE_TEMPLATE/BUG.md`](ISSUE_TEMPLATE/BUG.md) can be used by appending the following to a repo's new issue URL:
  - `?template=BUG.md`
  - For example: [`https://github.com/Centiq/.github/issues/new?template=BUG.md`](https://github.com/Centiq/.github/issues/new?template=BUG.md)
- [`PULL_REQUEST_TEMPLATE/ANSIBLE_ROLE.md`](PULL_REQUEST_TEMPLATE/ANSIBLE_ROLE.md) can be used by first constructing the PR comparison URL and then appending the following to it:
  - `?template=ANSIBLE_ROLE.md`
  - For example: [`https://github.com/Centiq/.github/compare/master...mybranch?template=ANSIBLE_ROLE.md`](https://github.com/Centiq/.github/compare/master...mybranch?template=ANSIBLE_ROLE.md)

Unfortunately, neither of these are available through the GUI, although the issue template selection options would be easy to add as predefined links in a repo's README.
