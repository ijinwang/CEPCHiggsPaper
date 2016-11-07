# CEPCHiggsPaper

This project documents CEPC Higgs measurement results and the physics interpretations, aiming for a paper to be published in Summer 2017. 
The paper will demonstrate the physics potential of the CEPC experiment and will be used as a reference for the CEPC CDR.

If you want to modify the paper draft, you need to register at https://github.com/, and send your username to jinwang.cepc@gmail.com for access rights.

Below is a very simple instruction on the usage of git only for those who never used git. 
This instruction resembles the svn and ignores some key features of git.

To download the repository (same as "svn co"), do:

$git clone https://github.com/ijinwang/CEPCHiggsPaper

Once you created or made any changes on file "modifiedfile.tex", do (similar as "svn ci -m" but not submit to the server yet):

$ git add modifiedfile.tex  (in svn you use "svn add" to stage a new file. While in git you use "add" to stage a new file or a new modification)

$ git commit -m "messages about your modifications"

or use "-a" to commit all the changes you made:

$ git commit -a -m "messages about your modifications"

If you want to push the commits you’ve done back up to the server (this plus previous step will serve as "svn ci -m"):

$ git push

If you want to update your local repository (same as "svn update"):

$ git pull


To make the best of git, please read:

https://git-scm.com/book/en/v2
