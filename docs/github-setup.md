# GitHub repository setup

The [Business Card project](https://github.com/users/kris1027/projects/10) tracks issues and pull requests for this repository. GitHub settings are applied directly; this file records them alongside the versioned templates.

## Issue forms and labels

- Bug reports use `.github/ISSUE_TEMPLATE/bug_report.yml` and apply the existing `bug` label.
- Feature requests use `.github/ISSUE_TEMPLATE/feature_request.yml` and apply the existing `feature` label.
- Blank issues remain available for other work. The bug form asks for test details and redacted evidence when reporting contact-form problems.

## Pull requests

`.github/pull_request_template.md` asks for a summary, verification, screenshots for visual changes, and a related issue where one exists. CI runs Lint, Typecheck, Test, and Build on pull requests to `main`.

## Repository metadata

The About description is `zaruszaj.pl: custom PC builds, technical help, and web development in Kraków.` Topics cover the services and the application stack. The website points to [zaruszaj.pl](https://www.zaruszaj.pl/).

## Main branch rules

The active `Protect main` ruleset targets `refs/heads/main`. It requires a pull request and the GitHub Actions `Lint`, `Typecheck`, `Test`, and `Build` checks, with the PR branch up to date with `main`. It blocks force pushes and deletion. Required approving reviews: zero, so the solo developer can merge after CI. No bypass actors are configured.

## Project

The public project has a description and README explaining its scope and status labels. Its `On track` update describes the live site without an invented deadline. New open issues and pull requests from this repository are automatically added to the project.
