# AstroUMD

Introduction to the use of the github AstroUMD organization. A top level documentation tree is also on GitHub Pages: https://astroumd.github.io/


## GIT for CVS users

In cvs you would
```
     cvs checkout URL
     ...
     cvs update
     ...
     cvs commit FILE
```
but this simple but direct commit back to the server is a now a two stage process in GIT:
```
     git clone URL
     ...
     git pull
     ...
     git commit FILE
     git push
```
In a (large) collaboration, this simple model of using git can still work if you
communicate, but there are better models.


## GIT using SSH

You can even avoid using places like github and bitbucket, or setting up your own gitlab, by using your ssh account into the department
computers. See http://www.astro.umd.edu/~teuben/git/ for a writeup. If you set your permissions correctly, it is also as safe as those
permissions.
     

## Some comments on using git

* Some common and recommended workflows can be found in the *git.txt* document

* a ***git clone*** does not preserve original timestamps (which e.g. CVS does). See   http://stackoverflow.com/questions/2179722/checking-out-old-file-with-original-create-modified-timestamps for some comments on this

* a ***git add*** of a new directory tree convieniently adds the whole tree, so ***git commit** will then commit the whole tree.

* After a ***git clone*** it doesn't seem to see other branches until you've been there?   (***git branch -r*** will list remote branches)

* If you delete a file, git will be upset. ***git checkout -- file***

