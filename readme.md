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
