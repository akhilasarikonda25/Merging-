>> create one file in main branch and added some code "app.py" 

now create one branch and open same file in newly created branch and added some more lines of code, branch name is dev2

After adding some more lines in new branch add the file and commit those changes 

Now switch to the main branch and open file and see the code newly added code should not add in main branch bcoz it is added in new branch 

now merge the dev2 branch from main use the following command 

git merge dev2 

and push the file to remote repository and finally check the file content in git hub 


Follow the below link to execute the commands 

[Jun 19 8_22 PM.txt](https://github.com/akhilasarikonda25/Merging-/files/11789416/Jun.19.8_22.PM.txt)

 
![Screenshot_1](https://github.com/akhilasarikonda25/Merging-/assets/133091109/fe24975a-fe29-4cdd-8637-601986fcdba6).

Git Rebase : 
1) suppose in master we are creating one projecr and that is very big it takes 1 week of time to complete , in that time dev 1 is writing and code and commiting , by that time in master branch created some commits by dev 2 1,2,3,4,5,6, commits and dev 2 will push the code to master branch 

2)  now dev 1 done with the coding now dev 1 is trying to push the code while pushing he might be face a lot of conflicts , to resolve those conflicts will use rebase concepts .

use the below commands 

 499  git init myproject
 
  500  cd myproject
  
  501  ls -al
  
  502  touch f1
  
  503  git status
  
  504  git add f1
  
  505  git commit -m "f1 added"
  
  506  git log
  
  507  touch f2
  
  508  git add f2
  
  509  git commit -m "f2 added"
  
  510  git log
  
  511  git branch mumbai
  
  512  git checkout mumbai
  
  513  git branch
  
  514  touch m1
  
  515  git add m1
  
  516  git commit -m "m1 added"
  
  517  git log
  
  518  git checkout master
  
  519  touch f3
  
  520  git add f3
  
  521  git commit -m "f3 added"
  
  522  git log
  
  523  git checkout mumbai

  524  git log
  
  525  git rebase master
  
  526  git log
  
  527  git checkout master
  
  528  git log
  
  529  git merge mumbai
  
  530  git log
  

All the files which are created in master , f1,f2,f3 and in branch m1 are merged in master and mumbai  branch .( with the help of rebase will push the branch file to the master ) .



Git Revert : 

1) Revert is nothing but removed a file , suppose created some files such as a, b, c, d and commited now if u want to remove the d file we can use git revert followed by commit id .

2) suppose if we want to remove b file all the files folowed by c,d are also deleted and it is also not the best practice to delete last but one file , make sure before commiting the code , code should be completed without any errors.

execute the below commands

  499  git log
  500  git revert 01e20c06e57260d7d2e98db23911b50c8234047e

Git reset :

1) There are 3 repo's in git

a) working directory 

b) Staging 

c) local rep

we are changing file from working dir to staging we use git add command 

we are changing file from staging to local repo will use git commit 

now if in case will modify a file and we add the file from working dir to staging area ,now developer wants to add some more content in that case he need to change the file from staging to working dir 
in that case will use git reset command 
Git reset command can be iused in 2 ways 
1)Git reset -- mixed

2)git rest --hard 

a) Mixed is used developer wants to modified a file and he want to continue development then he changed shifted file to staging to working dir at that time will use mixed.

b) hard is used developer mocved the file from working to staging he wants to stop the development , or else he dont want that file to move to the local repo in that case hard will be used 
