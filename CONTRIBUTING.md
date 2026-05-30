# How to contribute

Really appreciate your taking time checking this. ❤️

If you are looking for means of contacting me directly, please use the methods described under SECURITY for options.

## Bugs

Submit issues as you see fit. As of now, there is no template to adhere to.

- Add the error description
- Add the expected result
- Add some information about the context:
  - What were you trying to do (command, arguments, ...)
  - How did you try to do it (tool, version, ...)
  - Where did you do it (os, browser, ...)

## Ideas, Feature Requests

In most cases, Discussions are not enabled. Use issues instead.

Prepend the issue with `[FEAT] ` like in `[FEAT] please add support for service y to function z`.

## Testing

Only for large projects. Do not add dependencies to small projects that otherwise have none.

Document thouroughly. Either by commenting the code or with markdown sidefiles if there is a lot to consider / explain.

## Submitting changes

Submit Pull requests as you see fit. As of now, there is no template to adhere to.

- Add at least a small note that describes what you intend to change (and why)
- If applicable, link issues, you where trying to fix with it
- Submit as many PRs for different changes as you need. Packing unrelated commits into one PR prevents merging of all if only one is rejected.

Always add types to your contributions. See https://www.conventionalcommits.org/

Like `feat: support for service y`

If in doubt, use the following types:

- build: Changes triggered by automated workflows
- chore: Changes that affect the build system or external dependencies
- ci: Changes to our CI configuration files and scripts
- docs: Documentation only changes
- feat: A new feature
- fix: A bug fix
- perf: A code change that improves performance
- refactor: A code change that neither fixes a bug nor adds a feature
- revert: Revert a change
- style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- test: Adding missing tests or correcting existing tests

Optionally, add a scope if the change has a specific context:

Like `feat(z): support for service y`

## Coding conventions

Readability is key!

Especially, do not remove Whitespace just for the sake of getting less lines of code.
LOC is not relevant. It even breaks the advantages of git.
Checking in a one-line 10000 length json string without spaces and linebreaks is as helpful as adding a binary to the repository.

- Instead of "optimizing" LOC, make sure to not repeat yourself.
- Instead of "optimizing" LOC, separate your code into reusable parts (also divide and conquer).
- Use shortforms only when they help readability (most likely when working on text output)
- Enforce a maximum linelength only when it helps readability
- Keep it simple. Even if that means, dropping your hyper-efficient inline multi-nested multi-condition-loop in favor of a boring conditional function call.
- Do not use aliases (looking for an example? Check on the elephant in the room, powershell)
- If a high impact calculation requires to implement the most efficient solution that makes use of rarely used features, shortcuts, abbreviations or internal implementations, comment it in all detail.
- As for commenting, the more readable your code, the less additional commenting is needed.
- Even if the programming language does not enforce it, try working with / assigning types.
- Document return types for functions

More important points:

  * We indent using two spaces (soft tabs)
  * We avoid logic in views, putting HTML generators into helpers
  * We ALWAYS put spaces after list items and method parameters (`[1, 2, 3]`, not `[1,2,3]`), around operators (`x += 1`, not `x+=1`), and around hash arrows.
  * This is open source software. Consider the people who will read your code, and make it look nice for them. It's sort of like driving a car: Perhaps you love doing donuts when you're alone, but with passengers the goal is to make the ride as smooth as possible.

Thanks,
codeshell, TMW
