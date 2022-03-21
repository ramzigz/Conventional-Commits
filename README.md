# Conventional-Commits
## _Git commit message convention that you can follow!_

Each commit message consists of a **header**, a **body** and a **footer**.In this article we will focus only on the header of the commit's message.
The header has a special format that includes a **type**, a **scope** and a **subject**:

```sh
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

## type


**type** must be one of the following mentioned below!
- `build`: Build related changes (eg: npm related/ adding external dependencies)
- `chore`: A code change that external user won't see (eg: change to .gitignore file or .prettierrc file)
- `feat`: A new feature (new feature for the user, not a new feature for build script)
- `fix`: A bug fix (bug fix for the user, not a fix to a build script)
- `docs`: Documentation related changes
- `refactor`: A code that neither fix bug nor adds a feature. (eg: You can use this when there is semantic changes like renaming a variable/ function name)
- `perf`: A code that improves performance
- `style`: A code that is related to styling (formatting, missing semi colons, etc; no production code change)
- `test`: Adding new test or making changes to existing test


## scope

**scope** must be noun and it represents the section of the section of the codebase.
Example **scope** values:
- init
- runner
- watcher
- config
- web-server
- proxy

The **scope** can be empty (e.g. if the change is a global or difficult to assign to a single component), in which case the parentheses are omitted. In smaller projects such as Karma plugins, the **scope** is empty.

## subject
- use imperative, present tense (eg: use "add" instead of "added" or "adds")
- don't use dot(.) at end
- don't capitalize first letter

## Examples
Commit message with just type and description:
```sh
feat: allow provided config object to extend other configs
```
Commit message with type, scope, and description:
```sh
fix(middleware): ensure Range headers adhere more closely to RFC 2616

feat(lang): add Polish language
```
## Optional

Using emojis in your commit messages will be fun (😊) and cool (😎) in the first place.
[`Gitmoji`](https://gitmoji.dev/) is one of the fine guides you can refer to add emoji in our commits.


## References

- [https://dev.to/i5han3/git-commit-message-convention-that-you-can-follow-1709](https://dev.to/i5han3/git-commit-message-convention-that-you-can-follow-1709)
- [http://karma-runner.github.io/1.0/dev/git-commit-msg.html](http://karma-runner.github.io/1.0/dev/git-commit-msg.html)
- [https://www.conventionalcommits.org/en/v1.0.0/](https://www.conventionalcommits.org/en/v1.0.0/)
- [https://gitmoji.dev/](https://gitmoji.dev/)
