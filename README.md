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

#### 1.1.2 Git was NOT made up for tracking binary files

It's OK to be lazy once & do

`git add my-shit.[pkl|pth|npz]; git commit -m "typical useless fi commit msg"`

BUT, JUST AVOID making that a habit :please:
Especially when you work with other people. 

:warning: The same goes for machine-specific binaries aka don't do `git add *.[pyc|so|__pycache__]`

### 1.3 More resources

- [Samin's Git slides, SAICC-internal]()
