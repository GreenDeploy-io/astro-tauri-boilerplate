## How to rebase on upstream

### Using git commands

1. go to local repository `main` branch
2. `git remote add upstream git@github.com:ixartz/Astro-boilerplate.git` (one-time effort, skip if already have upstream)
3. `git fetch upstream` (assuming upstream as remote is created out of `git@github.com:ixartz/Astro-boilerplate.git`. see step 2 if not)
4. `git rebase upstream/main`


taken from https://stackoverflow.com/a/3903835/80353

### Using git tower

1. Right click on remotes and add new remote repository using `git@github.com:ixartz/Astro-boilerplate.git` (one-time effort, skip if already have upstream)
2. git fetch upstream
3. go to `main` branch and make sure it's HEAD
4. right click on `main` and `Rebase On` then select `upstream/main`