This repository contains the documentation for COGNOSYS.

Treat the GitHub repo as the "source of truth". GitBook is an excellent UI for editing and viewing the book.

The GitBook project has three workspaces: "documentation", "library", and "blog". Each one is synchronized to a directory in this GitHub repo (respectively, "documentation", "library", and "blog"). If the synchronization ever gets messed up, you can just make a new GitBook project and synchronize it to this repo.

"Library" is meant for any miscellaneous information or media you might want to keep on hand. The other 2 directories are self-explanatory.

Try forking the repo and adding a small contribution to a page of the documentation, then opening a pull request and I can practice and see how the merge workflow is.

I do not know but I think live synchronization will have to be turned off on GitBook since we will be multiple people editing, but I don't know for sure yet.

As far as I know currently, a GitBook is just a normal git repo, with three special (optional) files:

1. SUMMARY.md
2. SECURITY.md
3. README.md

