# Git Best Practices

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
