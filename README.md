# merge-conflict

<img width="457" alt="image" src="https://user-images.githubusercontent.com/95218914/225309419-5707ef9a-6474-4675-a259-94671ad881ed.png">

<img width="453" alt="image" src="https://user-images.githubusercontent.com/95218914/225309496-14d55120-a6df-4885-8032-0d09fd27f00b.png">
Step-wise:
Step-1: Add remote url to repository:

$ git remote add upstream https://github.com/HarshiniPR/merge-conflict.git

Step-2: Fetch changes from upstream master branch

$ git fetch upstream master
 
Step-3. Create new branch Feature 1 and switch to it

$ git checkout -b Feature1

Step-4. Merge master and Feature 1 branches

$ git merge upstream/master

Step-5. Push changes to Feature1 branch

$ git remote -v

$ git push upstream Feature1

Step-6. Create new branch Feature 2 and switch to it

$ git checkout -b Feature2

Step-7. Merge master and Feature 2 branches

$ git merge upstream/master

Step-8. Push changes to Feature 2 branch

$ git push upstream Feature2

Step-9. Switch to master branch

$ git checkout master

Step-10. Merge master and Feature 1 branches

$ git merge Feature1

Step-11. Merge master and Feature 2 branches

$ git merge Feature2

Step-12. Push changes to master branch

$ git push upstream master

Step-13. Push all branches to github

$ git push --all upstream
