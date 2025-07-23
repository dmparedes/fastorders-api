CONTRIBUTING.md
First, thank you for considering contributing to our project. We value your time and your interest in this project, and we appreciate every contribution that helps us improve it. Below are some guidelines for contributing.

Table of Contents
Development Environment Setup
Getting Started
Code Style
Documentation
Pre-commit Checks
Commit Messages
Pull Requests
Contact
Development Environment Setup
For a smoother development experience, we recommend the following extensions for VSCode and plugins for PyCharm:

VSCode Extensions:

Black Formatter
Code Spell Checker
dotenv
GitHub Actions
GitLens
isort
Live Preview
Live Server
Live Share
Makefile Tools
Markdown Preview Enhanced
Material Icon Theme
mypy
Path Intellisense
Prettier
Pylance
Python
ruff
YAML
PyCharm Plugins:

.env files
.ignore
Atom Material Icons
JSON Parser
Makefile Language
Material Theme UI
mypy
Rainbow Brackets
Requirements
String Manipulation
reStructuredText
Please refer to the respective extension and plugin documentation for installation and usage instructions.

Getting Started
Ensure you have cloned the repository. This will allow you to make and test your changes before pushing them for consideration.

Create a New Branch: Before you begin making changes, create a new branch for your work. This helps in isolating your feature or bugfix from the main codebase, making it easier to review and merge your contributions. Name your branch according to the feature you're working on or the bug you're fixing.

git checkout -b feature/AmazingFeature
or if you're fixing a bug:

git checkout -b bugfix/DescribeTheBug
Make Your Changes: After creating your branch, you can start making changes to the code. Ensure you're following our coding standards and guidelines for a smooth review process.

Commit Your Changes: Once you're satisfied with your changes, commit them to your branch. Be sure to write a clear and concise commit message, explaining what you've done and why.

git add .
git commit -m "A brief description of the changes"
Push Your Branch: After committing your changes, push your branch to the remote repository.

git push origin feature/AmazingFeature
Code Style
We follow the PEP 8 style guide for Python code. Please ensure your contributions adhere to this standard.

We recommend using a linter to check your code quality. You can check the documentation for Visual Studio Code or JetBrains PyCharm for more information.

For autocompletion, we recommend the TabNine plugin.

Documentation
When adding new code, please use docstring with reStructuredText format by adding triple double quotes """ after function definition. Add a brief function description, also for the parameters including the return value and its corresponding data type.

Pre-commit Checks
Before committing your code, you must have make installed on your system. For Windows users, we recommend using Chocolatey, a package manager that simplifies the process of installing and managing software.

To install Chocolatey, open an administrative PowerShell and execute:

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
After installing Chocolatey, you can install make by running:

choco install make
Once make is installed, you can run the following command in the root of your project to execute the checks defined in the Makefile:

make check
Please ensure that all checks pass before submitting a pull request.

Commit Messages
Please use clear and meaningful commit messages. This helps us understand the changes you've made and the reasoning behind them. If your commit resolves a specific issue, reference it in your commit message.

Structured Commit Messages
To maintain a clear and consistent commit history, we follow a structured format for our commit messages based on Conventional Commits. The format is as follows:

[type](reach): [description]
type: This indicates the nature of the change. Valid types include add, cut, fix, bump, make, start, stop, refactor, reformat, optimize, document.
scope: This specifies where the change was made, for example, database layer, UI, or API.
description: A brief, imperative summary of the change.
Example
fix(database layer): use async session for performance improvement
Pull Requests
Commit your changes to your branch.

git commit -m 'Add some AmazingFeature'
Push your branch to your fork of the repository on GitHub.

git push origin feature/AmazingFeature
Open a Pull Request from your fork to our repository. Please provide a detailed explanation of your changes and reference any related issues.

Contact
If you have any questions or need further clarification on anything, feel free to reach out. We are here to help!

Back to README.
