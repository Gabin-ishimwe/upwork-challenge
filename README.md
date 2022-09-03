# Git Challenge

There are two branches, add-echo and add-reverse. The goal of this challenge is to use git rebase to bring both commits onto master. When finished there should be no merge commits or branching. For example, git log on the master branch should look similar to this:

```bash
  /challenge-git master
⚡ git log
61a2c67 feat: add reverse route (David Guttman, 7 minutes ago)
2c2c5d6 feat: add echo route (David Guttman, 10 minutes ago)
dcc4c0b docs: add more instructions (David Guttman, 11 minutes ago)
...
```

# Solution

**Procedure**:

- Cloned this repository
- checkout on branch origin add-echo
- rebase and squash all commits on branch add-echo into one commit (feat: add echo route)
- checkout on branch origin add-reverse
- rebase and squash all commits on branch add-reverse into one commit (feat: add reverse route)
- returned on branch master
- run git rebase add-echo
- run git rebase add-reverse

**Git logs on Master branch**:

```bash
7ad9ffd (HEAD -> master) docs: add more instructions
e83e209 feat: add reverse route
7e86a19 (origin/add-echo, add-echo) feat: add echo route
6de0417 fix: change db path to project folder (#21)
8722c12 feat: log request auth info (#19)
30cdbf2 feat: add 401 status code for unauthorized requests (#17)
3f2732d fix: remove extra dep check (#15)
...

```

## Authors

- [Gabin Ishimwe](https://github.com/Gabin-ishimwe)
