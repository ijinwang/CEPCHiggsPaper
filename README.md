test modification 2

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

If you want to update your local repository (same as "svn update"):

$ git pull


To make the best use of git, please read:

https://git-scm.com/book/en/v2


test modification 1
