# CEPCHiggsPaper

This project documents CEPC Higgs measurement results and the physics interpretations, aiming for a paper to be published in Summer 2017. 
The paper will demonstrate the physics potential of the CEPC experiment and will be used as a reference for the CEPC CDR.

If you want to modify the paper draft, you need to register at https://github.com/, and send your username to jinwang.cepc@gmail.com.
An invitation email will be send to you and you will get full access rights after you accepted the invitation.


Below is a very simple instruction on the usage of git only for those who never used git. 
This instruction resembles the svn and ignores some key features of git.

To download the repository (same as "svn co"), do:

$git clone https://github.com/ijinwang/CEPCHiggsPaper

Once you created a new file or made any changes on existing file "modifiedfile.tex", do (similar as "svn ci -m" but not submit to the server yet):

$ git add modifiedfile.tex  (In svn you use "svn add" to stage a new file. While in git both new files and new modifications need to be staged with "add")

$ git commit -m "messages about your modifications"

or use "-a -m" to do the "add" and "commit" the same time with all the changes you made:

$ git commit -a -m "messages about your modifications"

If you want to push the commits you’ve done back up to the server (this plus previous step will serve as "svn ci -m" and it requests access rights):

$ git push

Before you upload your modifications, you should update your local repository first (same as "svn update"):

$ git pull

Note that "git pull" will fetch the most updated version from the server and will merge it with your local version.
It won't overwrite your local modification (same as "svn update"). 
You have to commit your changes first before "git pull", otherwise there will be warnings/errors.

There will also be warning if there are conflicts (the same line edited differently by you and others) between the local version and the version on the server, 
In this case, after "git pull " you can find all the information in the conflicted file. 
It will be shown as below with a conflict-marked area and the two conflicting blocks divided by a =======.

<<<<<<< HEAD (conflict marker begins, "HEAD" points to your repository)
your modification  (this is your version)
=======
modification on server (this is the version on server)
>>>>>>> branch-name (conflict marker ends, "branch-name" is the repository on servers)

You should edit the file and remove the whole conflict area with your prefers, and do "git commit -a -m" and "git push" to solve the conflicts.

test modification 5 If you want to discard your modification (make sure you want to do this!!) and restore previous version, use:

$ git checkout -- modifiedfile.tex

or discard all modifications:

$ git checkout -- .


To make the best use of git, please read:

https://git-scm.com/book/en/v2
