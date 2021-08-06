1. Adding changes to the last commit

Setup
```
echo "that last line I forgot" >> filename1.txt
```

How can you add this change to already created commit?
And without changing the 
What if the last commit was pushed? 
Can you push changes now?

2. Removing current changes

Setup
```
echo "A brand new file which is not tracked yet" > newfile.txt
echo "new changes to already tracked file" >> somefile.txt
```

How to remove all changes we've done to tracked files? And untracked?

3. Setting HEAD back - Completely removing commit

How to disregard a number of commits and change HEAD pointer?
What happens what you push such changes?

4. Undoing all commits that came from a merge

How to properly undo all of the commits from a branch?

5. Interactive rebase - squash

History is messy - one feature is spread across multiple changes
How to merge a number of commits into one?

6. Interactive rebase - squash with conflict
7. Interactive rebase - stoping for amends
