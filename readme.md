git clone https://github.com/miketestgit01/other
git submodule add https://github.com/miketestgit01/C-Programs.git

is the command used to bring create the submodule 
for this repository.


then,
git add -all 
git commit -m "added submodule"
git remote add origin https://github.com/miketestgit01/other
git push -u origin master

now,
check the local directory on your computer.
Notice the sub repo folders exist. but the contents of those folders are not there. that is because these too are submodules. a submodule is a pointer to a repository but not the repository itself. in order to get the contents of the sub sub modules (2xsub) you have to clone recursively to get all sub directories.

http://stackoverflow.com/questions/3796927/how-to-git-clone-including-submodules
command 

git clone --recursive git://github.com/miketestgit01/other
