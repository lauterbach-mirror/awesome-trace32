# Contributing

Share your expertise and contribute to the TRACE32 Community Projects! Here is how:

1) Make sure that your project adheres to the [Guidelines](#guidelines) below. :exclamation:
2) Create a pull request (PR) to add your project to the list of awesome TRACE32 projects (see [Pull-Request](#pull-request)). :rocket:
3) Wait for us to review your project and approve your PR. Please check the PR regularly or enable e-mail notifications in case we have questions. :eyeglasses:
4) Enjoy increased visibility and support from the TRACE32 community for your project! :tada:


## Pull-Request

We do not host the material, so please upload it to a platform of your choice.

On the top right of this repository's main page you can find the `fork` button. Please fork this project, add an entry for your TRACE32 Community Project to one of the awesome lists in `README.md` and create a pull request (we refer to the [forking workflow](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) often used in Open Source projects).

Make sure your description is short (desired: 100 characters or less) and that the link is pointing to your main repo branch rather than to a specific file.
Also consider the naming conventions as provided in the [Guidelines](#guidelines) below.


## Guidelines

- [Guidelines for Tutorials](#tutorials)
- [Guidelines for Scripts](#scripts)
  - [PRACTICE Scripts](#practice-scripts)
  - [Python Scripts](#python-scripts)
- [Guidelines for Tools](#tools)
- [Guidelines for Articles](#articles)

You have an awesome TRACE32 project that doesn't really fit those categories? Write an issue and describe your project a little. Maybe we can find a fitting category together or create a new one.

### Tutorials

Tutorials may be presentation slides, detailed blog posts or articles, or videos. The list entry should contain the **type of the presentation** accordingly (Slides/Article/Video). Tutorials may be in any **language**. However, make sure the title and the description is provided in English. Also mention the tutorial's language at the end of the list entry if the tutorial is not in English.

**Naming convention:** `[title](link)` **by** `author` **–** `type of material`**:** `short description (language if not English)`**.**

Example:
- [Debugging Linux on the FantasyBoard 42 with TRACE32](#) by My Company/Name – Video: Step by step guide on how to debug a Linux kernel module on the FantasyBoard 42 (German).


### Scripts

Scripts may serve any purpose, from board bring-up in Python to Tetris in PRACTICE.
Note the additional information regarding [PRACTICE](#practice-scripts) and [Python](#python-scripts) below.

**Naming convention:** `[title](link)` **by** `author` **–** `short description`**.**

Example:
- [Tetris in PRACTICE](#) by My Company/Name – A complete game of Tetris implemented in PRACTICE.


#### PRACTICE Scripts

Each PRACTICE script should contain a metadata header of the following form. It allows scripts to be found using the TRACE32 script search and provides fundamental information to collaborators.

```text
; --------------------------------------------------------------------------------
; @Title: [required]
; @Description:
;   [required]
; @Keywords: [optional]
; @Author: [optional]
; @Board: [optional]
; @Chip: [optional]
; @Copyright: (C) [year] [you/your company], licensed for use with TRACE32(R) only
; --------------------------------------------------------------------------------
```

Keys:

- `@Title`: Single line, should contain no more than 80 characters.
- `@Description`: May be multi-line, each line should contain no more than 80 characters. You can use this segment to document your setup. After reading the description a collaborator should have all information necessary to reproduce your setup.
- `@Keywords`: Keywords for search engines (not case sensitive).
    - When a script is placed into the demo folder `@Keywords` tags allow TRACE32 script search to find them.
- `@Author`: Your Name <your@email.address> (optional).
- `@Board`: Semicolon separated list of supported boards.
- `@Chip`: List of supported chips. Wildcards allowed (e.g., `XXX[A-Z0-9]`, `ARM[79]TDMI`, `MIPS*`, `C166?`).
    - `*` means any number of arbitrary characters (also no characters at all)
    - `?` means any single character
    - `[]` means any of the characters provided in the list of characters (using a hyphen can specify a range of characters, e.g., `[a-c]` is equivalent to `[abc]`)
- `@Copyright`: Use the current year and your/your company's name.
    - The copyright line must not report Lauterbach.

Note:

- If an optional metadata line does not apply omit the line entirely (don't leave blank).
- There must be no `$Id` line. This is an auto generated artifact of Lauterbach's version control system.


#### Python Scripts

Please make sure it is easy for other people in the TRACE32 Community to install and use your scripts by providing:
- the required Python version,
- the TRACE32 and Pyrcl version you used, and
- further required Python modules and their versions (e.g., use a pip requirements file).


### Tools

Open source software or hardware tools that extend the core functionality of TRACE32 or add new functions.

**Naming convention:** `[name](link)` **by** `author` **–** `short description`**.**

The field `author` is optional.

Example:
- [lauterbach-trace32-rcl](#) by Lauterbach GmbH – TRACE32 Remote Control for Python.

### Articles

Technical articles or blog posts are usually more in-depth and less educational compared to a tutorial.

**Naming convention:** `[title](link)` **by** `author` **–** `short description`**.**

Example:
- [Intricacies of the PRACTICE stack](#) by My Company/Name – An in-depth analysis of the PRACTICE stack and some neat tricks.
