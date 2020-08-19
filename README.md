setup: source the branch-man file in your bash profile.
view commands with `$ branch-man`

general workflow:

- create a branch with `branch/master/develop-n [name]`
- `branch-l` to see it
- when your changes are committed use `push` to push the branch, (automatically --set-upstream, and moves to in progress from local)
- with multiple branches use `checkout [p/l] [num]` to switch to a branch visible in `branch-l`

### COMMANDS:
- develop: switch to branch 'develop' and pull
- develop-n(ew) [name]: create a new tracked branch from branch 'develop'
- master-n(ew) [name]: create a new tracked branch from master
- hotfix-n(ew) [name]: redundant, same as above
- branch: show current branch name
- branch-save: write local/progress to file
- branch-init: fill local/progress from file
- branch-l: list current branches
- branch-n(ew) [name]: create a new tracked branch off current branch
- branch-c [regex]: remove all branches matching regex from tracking
- branch-a [branch]: add existing branch to tracking
- branch-m [new-name]: rename current branch, update tracking
- branch-na: stop tracking all branches
- prioritize [l/p] [num]: adds tracked branch to a list of priority branches
- normalize [regex]: removes mathing branch from the list of priority branches
- push: push current branch, create origin if not exists
- checkout [l/p/s] [num]: checkout (l)local, p(progress) s(priority) branch [num]
- set-feature: BROKEN sets current branch as 'feature' branch
- feature-n(ew) [branch-name]: BROKEN creates a new branch off of the current feature branch
