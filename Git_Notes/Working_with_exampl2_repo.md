Working with the example2 repository
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Creating a directory (myproject) > Initializing the git > Cloning the example2 repository > Creating some files in example2 > add & commit the files > pushing to main branch > creating new branch (newbranch)
> creating some files in newbranch > add & commit the files > push to newbranch > merging the newbranch to main > creating new branch (newbranch2) > creating some files in newbranch2 > add & commit the files > push to newbranch2 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   37  mkdir myproject
   38  cd myproject
   39  git init
   40  git clone https://github.com/ADR-SB/example2.git
   41  ls
   42  cd example2
   43  touch file1 file2 file3
   44  git add .
   45  git commit -m "myfirstcommit"
   46  git push origin main
   47  git branch
   48  git checkout -b newbranch
   49  touch new1 new2 new3
   50  git add .
   51  git commit -m "new_branch_commit"
   52  git push origin newbranch
   53  git checkout main
   54  git merge newbranch
   55  git push origin main
   56  git checkout -b newbranch2
   57  touch a b c
   58  add a b c
   59  git add a b c
   60  git commit -m "new_branch2abc"
   61  git push origin newbranch2
   62  git branch
   63  git remote -v
   64  git branch -a
   65  git pull
   66  git pull newbranch2
   67  git branch --set-upstream-to=origin/newbranch2 newbranch2
   68  git pull
   69  ls
   70  git pull
   71  ls
   72  git checkout main
   73  git pull
   74  git checkout newbranch
   75  git pull
   76  git pull origin newbranch
   77  history
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
