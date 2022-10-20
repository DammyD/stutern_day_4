# Topic: Collaborate with others in Git

- The main branch is supposed to be the "source of truth" for the project—changes to it should be carefully reviewed. Any change in origin/main becomes the new "source of truth" for anyone else working on the project, so we shouldn't just change it without some thought and review by others.
- Instead of working on main directly, let's branch off main into our own feature branch, and then merge those changes back into main.
- To begin, let's branch off of main and create our own feature branch to work on.
When you create a branch off of another branch, you create a copy of that branch at that point in time. You can now change this new branch independently of the original branch.
To try this out, let's make a new branch called chapter-2. To do this we use git checkout with the -b flag and the name we want the new branch to have:
- Notice that the terminal now shows us on the chapter-2 branch. Changes on the chapter-2 branch will not affect the main branch at all. We essentially have a new playground to make whatever changes we want to make without affecting main.
So we have a new branch, and for now that new branch is identical to main (we haven't made any changes yet). Next let's repeat what we've already done before and create a new file called chapter-2.txt, give it some content, and commit it:
- Now that we have a new commit on our chapter-2 branch, let's look the Git log and compare this new branch to main:
- We'll notice in the log that our latest commit is shown at the top, and our HEAD is again different from our origin. This again makes sense—we've made changes locally that aren't in GitHub.
Now we need to get our new changes into the main branch.
- There are a couple of ways to get our new Chapter 2 into the main branch and into GitHub, and the way we choose depends on the project and what workflow we're using to collaborate with others.
First let's talk about a couple different workflows we could use. 
  The first one is the most straightforward:
`Merge changes from chapter-2 into our local main branch`
`Push local main branch to origin/main`






