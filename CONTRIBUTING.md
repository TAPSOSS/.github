# Contributing to tapsOSS Projects
All tapsOSS projects are open source, and contributions are encouraged — whether it’s code, documentation, bug reports, or suggestions. 

This guide outlines the **general default contribution guidelines** for all tapsOSS repositories and will hold true unless otherwise specified in a repo’s README, CONTRIBUTING/CONTRIBUTING.md, or LICENSE.

## Quick Start

1. **Fork the repository**.
2. **Create a separate branch** for each change or new feature. Keep branches small and focused.
3. **Follow code style & documentation rules** outlined below.
4. **Update or add documentation** if your change affects usage or functionality.
5. **Submit a pull request (PR)** for review. Include a clear title and description of the changes.

## Table of Contents

- [Contribution Requirements](#contribution-requirements)
  - [File Names](#file-names)
  - [Emoji Usage](#emoji-usage-)
  - [Code Documentation In Code](#code-documentation-in-code)
  - [Comments In Code](#comments-in-code)
  - [Help Commands](#help-commands)
- [Commit Messages](#commit-messages)
- [Pull Request Checker](#pull-request-checker)
- [Author File/Credits](#author-filecredits)
- [Questions?](#questions)
- [License](#license)


## Contribution Requirements

### File Names

File names must be in snake_case (lowercase letters with `_` between words). Keep names concise and descriptive.

### Emoji Usage 😊

Emojis are strictly forbidden from being written into any code in any repository in this repo.
However, they are permitted to be used in documentation, READMEs, and author names.

It is recommended to use standard emojis to ensure the best compatibility.

### Code Documentation In Code

Every single function and class added to a tapsOSS projects needs a docstring containing a bare minimum of a 1-line comment explaining what it does in plain english and 
an additional line for each parameter/argument or return value explaining what they are/what they represent.
While required for any python files, it is heavily recommended to follow a styling similar to [Google's python docstring styling](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) in other filetypes too which looks like:
```
class Greeter:
    """
    A class that greets people.
    """

    def greet(self, name: str) -> str:
        """
        Return a personalized greeting.

        Args:
            name (str): The name to greet.

        Returns:
            str: A greeting string.
        """
        return f"Hi {name}!"
```

### Comments In Code

While not strictly required, it is heavily recommended to have a space after any single line comment markers in the code
(such as `# example comment` for an example of a single line python comment [comments in python are signified with the `#` character])

### Help Commands

While help commands aren't strictly required for all code/libraries, any command that can have a --help/-h flag to help explain potential use for a tool/function should be available when possible.

### Commit Messages

- Write commit messages in **English**.
- Keep them short and descriptive.
- Recommended format: `type: short description` (e.g., `fix: correct typo in player module`).

### Pull Request Checker

After sending in a pull request and filling out the template, you need to type "bot, check" (without the "s) for a GitHub actions bot to check your pull request for proper formatting, all the checkboxes, no emojis, etc. If it fails you'll need to type "bot, check" again after fixing things to check your commits again. Only once the bot is passing all the automated tests in this way will your code even have the chance to be merged.

### Author File/Credits

Anyone who has contributed any code, no matter how small or large, can add themselves to the dedicated `AUTHORS` file in each repo by adding their name and optionally their username
if they want to indented by one space. This will be used in any library/GUI to show a list of all the contributors to a project on top of the already existing list of contributors in the sidebar of the git repo and is likely what the average end user would see when looking for credits.

This is not strictly required by those who don't want their name attached to the project(s) in this way and can be added at any time (either alongside a pull request/merge or as its own pull request/merge).

To those interested, simply put your preferred name (and username afterward in parentheses) such as `Tristan (tapscodes)` or either simply `Tristan` or `tapscodes` depending on what you'd personally like in the next available open line in the AUTHORS file indented by a singular space.

## Questions?

If you have questions about contributing/a project in general:
- Open an issue for discussion
- Check existing issues and pull requests
- Review this contributing guide

## License

By contributing to any tapsOSS project, you agree that your contributions will be licensed under the same license as the project.

Most of the time (not always, check the `LICENSE` file of each repo to be sure) this is a BSD-3 License for code libraries and the GPLv2.0 License for other software projects.
Both of these licenses require attributing the original code base when using the code elsewhere, but the main difference is that the 
BSD-3 license allows use in closed source projects while GPLv2.0 requires projects to stay open source.
