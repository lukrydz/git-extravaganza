1. Adding changes to the last commit

```
echo "that last line I forgot" >> filename1.txt

git commit -am "new message" --amend 

# or without the message

git commit -a --amend --no-edit
```

What if the last commit was pushed? 
Can you push changes now?

2. Interactive rebase - squash

Setup
```
git checkout -b rebase-example

echo "file that gets the job done" > somefile.txt
git add somefile.txt
git commit -m "Add file doing some important work"


# moment of realization

echo "oops, file I forgot to add" > forgottenfile.txt
git add forgottenfile.txt
git commit -am "Add the forgotten file"


# moment of realization no 2

echo "Ok, I promise this is the last one" > lastfile.txt
git add lastfile.txt
git commit -am "Add the last file"


# see history

git log --oneline
```

History is messy - one feature is spread across multiple changes

**Squashing** is used to merge commits into another. We can merge our last commits into previous one.

```
git rebase -i master
```

3. Interactive rebase - squash with conflict
4. Interactive rebase - stoping for amends
5. Hard resets
