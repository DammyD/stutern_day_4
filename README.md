# Topic: Collaborate with others in Git

- The main branch is supposed to be the "source of truth" for the project—changes to it should be carefully reviewed. Any change in origin/main becomes the new "source of truth" for anyone else working on the project, so we shouldn't just change it without some thought and review by others.
- Instead of working on main directly, let's branch off main into our own feature branch, and then merge those changes back into main.
- To begin, let's branch off of main and create our own feature branch to work on.
When you create a branch off of another branch, you create a copy of that branch at that point in time. You can now change this new branch independently of the original branch.
To try this out, let's make a new branch called chapter-2. To do this we use git checkout with the -b flag and the name we want the new branch to have:
