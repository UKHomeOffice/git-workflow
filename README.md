# Git Workflow
A set of guidelines for using Git

## Workflow

```
$ git clone git@github.com:UKHomeOffice/git-workflow.git

$ cd git-best-practice

$ git checkout -b <branch-type>/<branch-name>
```

Develop

Stage chunks to be committed
```
$ git add -p
```

Commit staged changes
```
$ git commit -v
```

Fetch and rebase against the remote master branch
```
$ git fetch -p

$ git rebase origin/master
```

Push your committed changes to a remote branch
```
$git push origin <branch-type>/<branch-name>
```

Visit your Github repo and select open a pull request, selecting which two branches you into merge.

