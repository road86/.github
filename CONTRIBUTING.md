# road86 Contribution Guide

👋 **Hello there! Thanks for your interest in contributing!** 👋

The purpose of this guide is to ensure all contributors have a unified approach to contributing to all projects within the road86 space.

## Table of Contents

Looking for something specific? 🔍

- [road86 Contribution Guide](#road86-contribution-guide)
  - [Table of Contents](#table-of-contents)
  - [Create an Issue](#create-an-issue)
  - [Create a Pull Request](#create-a-pull-request)
  - [Linting, Formatting and Testing](#linting-formatting-and-testing)
  - [Commit Best Practices and Naming Conventions](#commit-best-practices-and-naming-conventions)
  - [Labels](#labels)
  - [Contact](#contact)

## Create an Issue

[{{back to navigation}}](#table-of-contents)

Our team uses 4 templates for creating issues across road86 repositories, and we would appreciate you also using these and filling them out with as much detail as you are able to provide. The templates include:

-   **Bug Report** – report any bugs whether technical or visual (the “bug” label will be automatically applied).
-   **Feature Request** – request any new features whether technical or visual (the “feature” label will be automatically applied).
-   **Enhancement Request** – request any enhancements whether technical or visual (the “enhancement” label will be automatically applied).
-   **Test Request** – request a new test not currently available (the “test” label will be automatically applied).

**NOTE:** Please remember to first determine which repository the issue should be raised in, then [search the road86 repositories](https://github.com/search?q=user%3Aroad86+is%3Aissue) to ensure the issue you want to open is not already open or even been previously closed!

The process of reporting a found **Security Vulnerability** is different to the above. You should only report this problem to the team via an email report by contacting us at [security@road86](mailto:?subject=[GitHub%20-%20Security%20Vulnerability]) and we would apprieciate you also including as much detail as you are able to priovide. Please refer to the [road86 Security Policy](https://github.com/riad86/.github/blob/main/SECURITY.md) 🔒 for further details, including a content guide to create an in-depth report.

**NOTE:** If you try to report a found **Security Vulnerability** via the normal GitHub issue process, you will be redirected to the [road86 Security Policy](https://github.com/road86/.github/blob/main/SECURITY.md) 🔒 instead of an issue template. So feel free to access the [road86 Security Policy](https://github.com/road86/.github/blob/main/SECURITY.md) 🔒 either way, which ever suits your workflow!

## Create a Pull Request

[{{back to navigation}}](#table-of-contents)

The **Pull Request** template should be filled out as much as possible. Your pull request should include a summary of the changes you have made and your motivation behind them. Please list any dependency changes, added tests, documentation changes, database changes (if applicable) and complete our checklist to ensure you have completed all the necessary steps.

Please remember to first [search the road86 repositories](https://github.com/search?q=user%3Aroad86+is%3Apr) to make sure the pull request you want to create is **not already open or closed**!

After you submit your pull request, please assign at least one reviewer and assign any [labels](#labels) you think are applicable. Please also verify that all status checks are passing. If for some reason they are failing and you believe it’s unrelated to your change or unsure why, please leave a comment on the pull request explaining this and someone on the road86 team will further investigate.

## Linting, Formatting and Testing

[{{back to navigation}}](#table-of-contents)

For linting and formating our team uses [flake8](https://github.com/PyCQA/flake8) and [black](https://github.com/psf/black) for linting and auto-formatting our Python code alongside [pytest](https://docs.pytest.org/en/6.2.x/) for our Python code tests, or [eslint](https://eslint.org) and [prettier.io](https://prettier.io) for linting and auto-formatting our TypeScript code alongside [jest with react-testing-library](https://jestjs.io/docs/tutorial-react) for our TypeScript code testing.

For system and visual testing our team uses [BrowserStack](https://www.browserstack.com) – specifically [Automate with Selenium](https://www.browserstack.com/automate), and [Percy](https://www.browserstack.com/percy) Snapshots together to test at scale the platform works as antipicated.

_Any further or alternative specifics and configuration files can be found in each of our repositories._

If you create a pull request, your contributed code will automatically be linted, formatted and tested by the GitHub Action we have set up. New code should always use the same linters and formatters the road86 reposorities currently use. We would also really appreciate new code to come with new tests, where appropriate, to be run against all existing tests!

## Commit Best Practices and Naming Conventions

[{{back to navigation}}](#table-of-contents)

Our commit best practises encourage creating small and frequent commits with clear log messages while editing the source code. This ensures commits are focused and any changes are easily understood and revertible if something goes wrong.

Commit messages should indicate the type and include a short summary of the commit using the following conventions:

-   **feat**: The new feature you're adding to a particular application.
-   **fix**: A bug fix.
-   **build**: Development changes related to the build system (involving scripts, configurations or tools) and package dependencies.
-   **test**: Everything related to testing.
-   **docs**: Everything related to documentation.
-   **chore**: Regular code maintenance and/or style changes/formatting.

For example, “feat: add new icon svg file” or “fix: lint errors”.

One-line commit messages are perfect for small changes, but larger changes should include a paragraph describing what has changed and what is its impact alongside.

## Labels

[{{back to navigation}}](#table-of-contents)

Each issue and pull request should be assigned one or multiple labels depending on the content. We actively encourage all contributors to attach labels onto any issues and pull requests they open to categorise tasks and problems, making it visually easier to find and understand which ever task or problem is being handled in each issue and pull request.

Our repositories have 4 label categories which are subdivided into their own labels.

**Build Updates** (light grey)

-   [dependencies](https://github.com/search?q=user%3Aroad86+label%3Adependencies+is%3Aopen) – Pull requests that update a dependency file.
-   [deployment](https://github.com/search?q=user%3Aroad86+label%3Adeployment+is%3Aopen) – Anything relating to deployment.

**Problem** (red)

-   [bug](https://github.com/search?q=user%3Aroad86+label%3Abug+is%3Aopen) – Something isn’t working or looking right.
-   [question](https://github.com/search?q=user%3Aroad86+label%3Aquestion+is%3Aopen) – Further information is requested and/or required.

**Improvement** (blue)

-   [feature](https://github.com/search?q=user%3Aroad86+label%3Afeature+is%3Aopen) – New feature request.
-   [documentation](https://github.com/search?q=user%3Aroad86+label%3documentation+is%3Aopen) – Documentation-related request.
-   [test](https://github.com/search?q=user%3Aroad86+label%3Atest+is%3Aopen) – Anything related to testing or tests.

**Inactive** (black)

-   [wont-fix](https://github.com/search?q=user%3Aroad86+label%3Awont-fix+is%3Aopen) – This will not be worked on in the near future.
-   [duplicate](https://github.com/search?q=user%3Aroad86+label%3Aduplicate+is%3Aopen) – This issue or pull request already exists.

These labels are mostly consistent across road86 repositories to make it easier for everyone while working across multiple. If you forget this don't worry, when you open your issue or pull request each label has a description.

## Contact

[{{back to navigation}}](#table-of-contents)

Need some help? 🤔 Have a question? 🧠 \
Reach out to the appropriate Slack channel.
