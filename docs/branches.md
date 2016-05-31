#Branches

## Naming conventions

- Separate the parts of a branch name with a forward slash
- Use hypens rather than camelcase
- Keep the name relevant, if the purpose of the code changes, change the branch name: `git branch -m <new-branch-name>`

### Type

There should be two main types of branch; 'feature' and 'bugfix', and both are pretty self-explanatory. If you want to be more specific you can also use 'improvement' or 'enhancement' when it is neither a feature nor a bugfix the branch has been created for.

### Reference

When you've established what problem you are trying to solve and therefore named the first part, and "type", of your branch, add a reference. A reference should be in the form of a ticket number, for instance a Jira or Github issue number such as, abc-01 or #01, respectively. This makes it easy for anyone to link the branch and code to an issue.

### Description

Thirdly, add a concise description. The description must be short, useful and preferably hyphenated for readability. A good example of this would be: `.../add-age-field`

### Examples

#### Good

`feature/abc-10/add-age-field`

`bugfix/xy-34/remove-redis`

#### Bad

`feature/refactorAllTheThings`

`joe-smith/stuff`
