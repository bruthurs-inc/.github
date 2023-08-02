# How .github Works

Repositories hosted on GitHub have the concept of a `.github` directory, which holds files that inform the interaction with / displaying of data in that repository on github.com (things like templates, code ownership, workflows, etc).

However, when `.github` is the name of a _repository_ within the organization (versus the name of a directory inside an individual repository), the files in that repository will become the default information for interacting with and displaying data for _every repository in that organization_.

This allows us to provide things, like a default Pull Request Template, that pre-populate every Pull Request created in every repository.

> Note: if unique and specific info is desired for an individual repo, one can still use the `.github` dir within that repo to store that info. The repo-level `.github` dir will always trump the org-level `.github` repo's info.

Some cool things we can add at the org-level, or the repo-level, are:

1. CODEOWNERS -- determines which specified users/teams to auto-tag as a Reviewer in opened PRs.
2. Issue Template -- a template that pre-populates new issues with guiding questions.
3. Pull Request Template -- a template that pre-populates new pull requests with guiding questions.
4. README Template -- a template that pre-populates READMEs in new repos. Use this for guiding the setup of a new README, or to include top-level information in every README.
5. Workflows -- pre-built workflows for boards, code, and even new repo creation.
6. Community Health Files -- things like licenses, organizational info, links, etc.
