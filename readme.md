create one file in main branch and added some code "app.py" 
now create one branch and open same file in newly created branch and added some more lines of code, branch name is dev2
After adding some more lines in new branch add the file and commit those changes 
Now switch to the main branch and open file and see the code newly added code should not add in main branch bcoz it is added in new branch 
now merge the dev2 branch from main use the following command 
git merge dev2 
and push the file to remote repository and finally check the file content in git hub 

    vi integer.py
  523  git checkout dev2
  524  vi integer.py
  525  vi integer.py
  526  git add integer.py
  527  git commit -m "added content in dev2 branch"
  528  vi integer.py
  529  git checkout master
  530  vi integer.py
  531  git merge dev2
  532  vi integer.py
  533  git merge dev2
  534  git add integer.py
  535  git commit -m "add"
  536  git push
 To ignore the files we wil use create file with some extension and will ignore the file 
>> 538  touch xyz.pyc
  539  git status
  540  vi xyz.pyc
  541  vi .gitignore
  542  git status

![Screenshot_1](https://github.com/akhilasarikonda25/Merging-/assets/133091109/fe24975a-fe29-4cdd-8637-601986fcdba6)
