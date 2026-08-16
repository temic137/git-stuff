# My Learning Log

## About This Project
I'm learning Git and version control to track my work.

## Goals
- Understand how commits work
- Learn branching and merging
- Push my work to GitHub
## What I Learned Today

- Git is like a time machine for your files
- Every commit is a snapshot you can go back to
- Git tracks changes to files over time
- Branches let you experiment without affecting the main project
- You can merge branches back together when ready


## Reset

- git reset --soft HEAD~1: undo last commit, keep changes staged
- git reset --mixed HEAD~1: undo last commit, keep changes in working directory (default)
- git reset --hard HEAD~1: undo last commit and discard all changes (dangerous!)
- Only safely use reset on commits that haven't been pushed


## Bisect

- git bisect start: begin a binary search session
- git bisect bad: mark current commit as containing the bug
- git bisect good <ref>: mark a known-good commit
- Git checks out middle commits; you test and mark good/bad
- git bisect reset: end the session and return to original HEAD
