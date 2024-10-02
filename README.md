# [Software Development Tips For Scientist](https://github.com/escorciav/dev-tips-for-scientist)

Scientists are great, right?
Einstein, M. Curie, Fermi, etc.

Not all though!
Especially when a field gets trending &/Or crowded (Nuclear Physics => Nuclear Engineering, ML Science => ML Engineering, etc.)

But, hopefully a/some? colleague of yours got trained as
- Scientist
- Engineer

## 1. Git Tips

### 1.1 Day to day tips

#### 1.1.1 Git was NOT made up for tracking binary files

It's OK to be lazy once & do

`git add my-shit.[pkl|pth|npz]; git commit -m "typical useless fii commit msg"`

BUT, JUST AVOID making that a habit :please:
Especially when you work with other people. 

:warning: The same goes for machine-specific binaries aka don't do `git add *.[pyc|so|__pycache__]`

### 1.2 Tips to NOT get entangled in branches

#### 1.2.1 Branch & commit

Branch out of the central development branch (or backbone), and sync often.

Usually the main branch is called `main` or `master`.

```
git checkout main
git chechout -b new-awesome-feature
git commit
git push
```

> In doubt about the main dev branch? ask the project owner, admin, or maintainers  :)

#### 1.2.2 Setup your git config

Update your local config such that you pull with rebase & push to the corresponding branch.

You can config git to do so by default in your git-config, usually placed on `~/.gitconfig`, my looks alike

```text
[push]
    default = current
[pull]
    rebase = True
```

You can also do it per repo or global.

> TODO: contribution of terminal commands to do it is welcome

### 1.3 More resources

- [Git workflow](https://git-scm.com/docs/gitworkflows#:~:text=gitworkflows%20-%20An%20overview%20of%20recommended%20workflows%20with%20Git.%20SYNOPSIS.)

- [Samin's Git slides, SAICC-internal]()
