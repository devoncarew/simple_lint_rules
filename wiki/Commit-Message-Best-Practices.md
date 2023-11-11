# Commit Message Best Practices

> [!IMPORTANT]
> The contents of this doc were copied from our wiki and have not yet been
> confirmed to be current and up-to-date. When this doc is next reviewed and
> updated please remove this comment.

1. First line is a capitalized, short (50 chars or less) summary,
   * Please include the component for which the change is being made in the first line
     * **[Analyzer]** short (50 chars or less) summary
     * **[dart2js]** short (50 chars or less) summary
     * **[CFE]** short (50 chars or less) summary
     * **[CoreLib]** short (50 chars or less) summary
     * **[ddc]** short (50 chars or less) summary
     * **[VM - Runtime]** short (50 chars or less) summary

1. **Always** add a blank line before more information. Many git tools assume this layout.

1. More detailed explanatory text, if necessary. Wrap it to about 72 characters or so.

1. When linking to an associated GitHub Issue
  * **DO NOT** put `Issue 234` in the title
  * **DO** Use the full GitHub URL to the issue - this ensures that the issue is clickable in Gerrit
  * **DO** Use GitHub notation to auto-close bugs on commit
    * This: `Closes https://github.com/dart-lang/sdk/issues/25595`
    * Not this: `BUG=https://github.com/dart-lang/sdk/issues/25595`
  * If you don't want to delete the `BUG=` boiler plate, at least add a space after the `=`. This ensures that the issue link is clickable in Gerrit.
  
5. Write your commit message in the present tense:  "Fix bug" and not "Fixed bug." This convention matches up with commit messages generated by commands like git merge and git revert.

## Example

```
[VM - GC] Summarize changes in 50 chars or less

More detailed explanatory text, if necessary. Wrap it to about 72 characters or so. In some
contexts, the first line is treated as the subject of an email and the rest of the text as the
body. The blank line separating the summary from the body is critical (unless you omit the
body entirely); tools like rebase can get confused if you run the two together.

Closes https://github.com/dart-lang/sdk/issues/1

Further paragraphs come after blank lines.

- Bullet points are okay, too

- Use a hyphen or asterisk, followed by a single space.

- Use a hanging indent for 
  longer lines
```
## See also:

* [Closing issues via commit message (GitHub)](https://help.github.com/articles/closing-issues-via-commit-messages/)
* [A Note About Git Commit Messages](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)