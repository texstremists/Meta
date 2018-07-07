# How to contribute





### Table of contents

[How can I contribute?](#how-can-i-contribute)

[Contribution rules](#contribution-rules)

- [Essential rules](#essential-rules)

- [Soft rules](#soft-rules)



## How can I contribute?



Q: I don't want to read this whole thing, I just have a question.

A: Let us discuss it on [Gitter](https://gitter.im/GeM-ECN/Lobby).



## Contribution rules

The following set of rules are rather guidelines than strict rules. If you have objections or recommendations, feel free to open an issue in the [Meta repository](https://github.com/texstremists/Meta).

The two places you can contribute to:

- repository tree
- wiki pages



### Essential rules

1. Do **not** create new repositories

   Almost all topic fits into one of the existing repositories. If you really think your proposed topic is very different, let us discuss it in the [main room](https://gitter.im/GeM-ECN/Lobby).

2. Do not create new top-level folders in an existing repository unless you are sure that this is really a new topic

   If in doubt, ask other people in the respective chat room. Create low-level folders if your contribution consists of several files.

  The rationale behind the first two rules is that your contribution probably already fits in an existing repository/directory. Moreover, moving files with git messes up the log and gives extra work to the admin. As the number of contributions increase, a logically structured repository is a must.
3. Do not upload anything illegal

4. Respect the copyright

   If your work includes code chunks from external sources, attach the original license.

5. Prefer text files to binaries

   - Very small files (e.g. tiny png-s) are fine to be versioned. 
   - Output files (e.g. `*.pdf,*.exe`) should not be in the repository, unless users may not be able to compile it (e.g.  fontastic.pdf) or there is no way to store it remotely and permanently. Alternatives:
      - use a cloud-based *permanent* storage (e.g. [imgur](https://imgur.com/))
      - use [git LFS](https://help.github.com/articles/configuring-git-large-file-storage/)

6. All documentation, file names, comments must be written in English

   English is the lingua franca in science and programming.



### Soft rules <a name="rules-soft"></a>

1. Learn the basics of git. With administrator rights, you can cause serious damage to the repository, so be careful.

2. Git commit guidelines

   - The commit messages should be terse but understandable: not too short and not too long. One sentence is usually enough (see the next advice).

   - Commit one single change (mainly important in codes); do not make enormous changes in one commit.

3. Folder naming conventions (to be agreed). Make it explicit, avoid things like *test2-v4.cc* 

4. Coding conventions (aka styleguides)

   Since most of the files are from individuals, no coding convention is needed unless working in a team.

   - Keep it minimal to the intended purpose

   - Comment everything not obvious (but do not overuse commenting: rather use descriptive variable/function/class names)

   - If your file needs unusual compilation, mention it at the top (e.g. LuaLaTeX, index, very recent versions of whatever)

5. If (part of) your solution uses sources, always cite them
   It gives credit to the author and helps the interesting reader delve into the topic.

6. Strive for precise writings

   Use spell checkers. Do not use informal language in the wiki pages and the program codes. Smileys and slang language is appropriate only on Gitter.

7. Stick to the minimum both in the wiki and in the code when describing something

   It helps concentrating on the issue to be presented.

8. Create a structure when writing new topics into the wikis

   It helps others understand what goes into that section. Follow the existing structure when 

9. Make use of Markdown's syntax

   - For tips, see [our guide](https://github.com/texstremists/Meta/wiki/Markdown).

   - Use hyperlinks amply to refer to external sources

   - Use hyperlinks for internal references (e.g. table of contents)

   - For longer markdown files, create a table of contents (TOC)

   - Use comments to make TODO notes (they are not displayed)

10. Test your code before commiting it

    - include the tests too; they *prove* that your code works as intended
    - for very simple codes, tests are not necessary (hence avoiding to create sub-folders)
    - test against corner cases
    - whenever a new feature is implemented, run your test suite to see if all tests pass
    - [TDD](https://en.wikipedia.org/wiki/Test-driven_development) is a recommended and powerful agile software development technique

11. Prefer spaces to tabs for indentation
    Most editors can automatically convert tabs to spaces.

12. Do not write variables, comments and file name all capital letters