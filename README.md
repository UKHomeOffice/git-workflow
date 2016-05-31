# Git Workflow

A set of guidelines and principles to help define your workflow with Git

## The quick example

Make a local copy of the code
```
$ git clone git@github.com:UKHomeOffice/<repo_name>.git
$ cd <repo_name>
```

Create a branch [using these detailed naming guidelines](./docs/branches.md#naming-conventions)
```
$ git checkout -b <branch_type>/<branch_name> (E.g. feature/add-feature1 or feature/ABC-1)
```

**This is the part where you make the changes relevant to the ticket and new branch name you are working in**


Add your changes to be committed. The `-p` (`--patch`) gives you the opportunity to accept (`y`) or decline (`n`).
```
$ git add -p
```

Commit staged changes. The `-v` (`--verbose`) will open an editor showing an overview of your changes, so you can be super-descriptive when writing your [commit message](https://github.com/alphagov/styleguides/blob/master/git.md).
```
$ git commit -v
```

Fetch and rebase against the remote master branch. `-p` (`--prune`) removes remote-tracking references that no longer exist on the remote.
```
$ git fetch -p

$ git rebase origin/master
```

Push your committed changes to a remote branch
```
$ git push origin <branch_type>/<branch_name>
```

- Visit your Github repo and select "New pull request", selecting which two branches you intend to merge. This will usually be your feature branch and master. Master will be preselected as the branch to merge into.

- [Follow these guidelines](https://github.com/alphagov/styleguides/blob/master/git.md) to help describe the nature of your pull request, particularly the use case and the objectives it attempts to achieve.

- Assign the pull request to a *qualified* member of your development team for a technical review.


