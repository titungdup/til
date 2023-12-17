**Git Merge**

Git merge creates a new commit in the main branch that ties the histories of both main and feature branches.

Git merge is non-destructive. Neither the main nor the feature branch is changed.

**Git Rebase**

Git rebase moves the feature branch histories to the head of the main branch. It creates new commits for each commit in the feature branch.

The benefit of rebase is that it has _linear commit history_.

Rebase can be dangerous if “the golden rule of git rebase” is not followed: Never use it on public branches!
