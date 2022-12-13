# Git Best Practices

## Keep Commits small
### Easier Debugging
Imagine that several months from now you find a bug. You jump to a previous commit where you assume the bug did not yet occur. Depending on whether the bug has already occurred or not, you jump forward or backward in the commit history. Finally you find the commit that caused the error. If your commit is of a manageable size and contains only one central change instead of many changes to different components, you can identify and fix the cause of the bug very quickly.
### Easier Reverting of changes
If changes need to be rolled back, it is easier to roll back an entire commit instead of reverting changes with a new commit.
### Better Change Logs
Change Logs can be generated automatically. If the commited changes are small and specific the generated change logs are far better in quality.
### Easier to review and discuss
Time is valuable. If you handover a big commit to a collegue for review you won't make him happy because your collegue has to invest more time to understand what the changes are for. It is not uncommon for commits to be simply waved through in such cases. This means that the goal of a code review is missed and poor code quality is possibly introduced into a production system.

## Conventional Commits
Make use of [conventional commits](https://www.conventionalcommits.org/).

#### Commit Types
```
feat – a new feature is introduced with the changes
fix – a bug fix has occurred
chore – changes that do not relate to a fix or feature and don't modify src or test files (for example updating dependencies)
refactor – refactored code that neither fixes a bug nor adds a feature
docs – updates to documentation such as a the README or other markdown files
style – changes that do not affect the meaning of the code, likely related to code formatting such as white-space, missing semi-colons, and so on.
test – including new or correcting previous tests
perf – performance improvements
ci – continuous integration related
build – changes that affect the build system or external dependencies
revert – reverts a previous commit
```
### Additional resources
- [How to Write a Git Commit Message - by cbeams](https://cbea.ms/git-commit)

### Commit Message
Use the imperative mood in the subject line

Imperative mood just means “spoken or written as if giving a command or instruction”. A few examples:

Clean your room

Close the door

Take out the trash

A properly formed Git commit subject line should always be able to complete the following sentence:

If applied, this commit will **your subject line here**
