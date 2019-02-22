# Coding standards

## Overview
Coding standards: Some hate it :( Some love it! So who is right? Probably an informed decision as *a team*, following basic industry standards but not too tight. Considering that an IDE can automatically clean your code for you, as can a simple command from the command line (unless you did something stupid which you need fix), it would seem to be low cost and provide value. 
While there are many things that need to be considered to have clean code written across a team or project, one item that is fairly simple to implement is making sure the code follows *industry established* standards. Each language has its standards that can be fine tuned and implemented across the team.
This has a few benefits:
1. Insures that the code does not have basic errors (no one will **ever** push code missing a breaking semicolon)
2. Improves code readability 
   - The code will be pretty, neat and conforms to standard
   - Creates code style uniformity across the team
   - The above makes it much easier for any dev read anyones code

### Linting vs sniffing
- Code linting -  generally this refers to the process of look for and fixing of formatting, syntax errors and obvious bugs
- Code sniffing - a code sniffer is used more generally to inspect code for anything that you want, this is used to enforce coding standards 

## What and how

### What to look for
- Formatting standards
- Syntax errors
-  Commenting standards
   - Ensure that code is properly commented (e.g. following DocBlock standards)

### How to inspect and fix
- IDE - just setup you IDE to use the standards implemented by your team
- Command line - run a command from the command line to make your code pretty 
- GIT hook - a git hook can run above said commands on git commit, this insures that you never push sub par code
- CI - as matter of insurance linting vs sniffing should run in deploy script, this way if there is an issue it will not deploy

## Links
Yes these links are PHP slanted :/
- [ESLint](https://eslint.org/) // Lint for JavaScript
- [Automated code reviews](https://www.codacy.com/)
- [PHP CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) // Code sniffer for PHP
- [StyleCI](https://styleci.io/) // Automatically fix the style of your PHP, JS and CSS code.
- [GrumPHP](https://github.com/phpro/grumphp) // A PHP code-quality tool (uses Git hook)
- [Git Hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) // Setting up Git hooks
- [PHP Mess Detector](https://phpmd.org/about.html)
