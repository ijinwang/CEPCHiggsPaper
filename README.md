# CEPCHiggsPaper

This project documents CEPC Higgs measurement results and the physics interpretations, aiming for a paper to be published in Summer 2017. 
The paper will demonstrate the physics potential of the CEPC experiment and will be used as a reference for the CEPC CDR.

Below is a very simple instruction on the usage of git for those who never used git. 
This instruction resembles the svn and ignores some key features of git.

First, you need register on https://github.com/, and send your username to jinwang.cepc@gmail.com for access rights.

To download the repository (same as "svn co"), do:

$git clone https://github.com/ijinwang/CEPCHiggsPaper

Once you made any changes on file "modifiedfile.tex", do (similar as "svn ci -m" but not submit to the server yet):

$ git add modifiedfile.tex
$ git commit -m "messages about your modifications"

or use "-a" to commit all the changes you made:

$ git commit -a -m "messages about your modifications"

if you want to push the commits you’ve done back up to the server (this combined with previous step will serve as "svn ci -m"):

$ git push

if you want to update your local repository (same as "svn update"):

$ git pull


to fully benefit from the git advantages, please read:

https://git-scm.com/book/en/v2
