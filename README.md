# Git-Flow
All required info for git flow and git management


## Remove all stale branches from local
1. `git fetch --prune`
2. Then, to delete local branches which have been removed from remote(which we got from above command):
   `git branch --v | grep "\[gone\]" | awk '{print $1}' | xargs git branch -D`
