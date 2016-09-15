##Instructions to build a repository like this for yourself

git clone https://github.com/miketestgit01/Submodule-Example

the command used to bring create the submodule     
for this repository.

git submodule add https://github.com/miketestgit01/C-Programs.git




then,


git add -all 


git commit -m "added submodule"

git remote add origin https://github.com/miketestgit01/Submodule-Example

git push -u origin master

now,

check the local directory on your computer.
Notice the sub repo folders exist. but the contents of those folders are not there. that is because these too are submodules. a submodule is a pointer to a repository but not the repository itself. in order to get the contents of the sub sub modules (2xsub) you have to clone recursively to get all sub directories.

http://stackoverflow.com/questions/3796927/how-to-git-clone-including-submodules
command 

#Manipulations not requiring any work.
##Clone to your local computer

git clone --recursive https://github.com/miketestgit01/Submodule-Example.git

note: https://github.com/miketestgit01/Submodule-Example.git
(will not copy all files)

##Delete from your local computer through terminal

to delete locally.
rm -rf localdirectoryname
