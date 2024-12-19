WHAT IS GIT
 Git is a version control system (VCS). It helps developers track changes in their codebase over time, collaborate with others effectively, and manage different versions of their projects. Basically, Git is like a time machine for your code, aur haan, open-source hai, toh free hai!
 
GIT CONFIGERATION

1. git config --global user.name "shiv"
2. git config --global user.email "ss1364551@gmail.com"
3. git config --global core.editor "code --wait"
4. git config --global core.autocrlf "input"

to edit your configeration _
 git config --global -e

------------------------------
STAGES -
 U - UNTRACKED (git is not managing your project and neither tracking)
 A - ADDED & STAGED (now git knows the file exists)
 C - COMMITED (now git is trackin you file)
-------------------------------

COMMAND YOU NEED TO KNOW -
git log --oneline => to know currnet status of saved point
 -  git log bataata hai saare commit histories
git status -s => kon si file kis stage me hai
 -  git status srf unka status bataayega jo files committed nahi hai ya fir commit hone
ke baad change ki gayi
 - git status batata hai file ke changes ke baare me and uske stage ke bare me , before commit and after commit.
THINGS YOU NEED TO KNOW - 
-if you want to hide any file from the git you have to make .gitignore file and in the file mention the file name you want to hide , with this now git always ingore and do not tract it.

-------------------------------

AFTER GIT INSTALLTION AND CONFIGERATION 

=> FIRST WE HAVE TO DO IS - making git available in your project.   

IN VS CODE -
    go to the SOURCE CONTROL - and initialize repository

=> SECOND WE HAVE TO DO - making a checkpoint or saved point
  - adding file  - create any file bro
  - staging them - means add them in to the staged changes by going on you source controll , when you do that the stage of file became A.
  - commiting them

=> THIRD - going back to some previous saved point
    logging everythig
    reverting back to the previous saved point


   - reset has three main options:
    --soft
    --mixed
    --hard  

   1. git reset --hard HEAD~1 => Moves the HEAD to the specified commit and discards all changes in the staging area and working directory.
⚠️ This is destructive! You'll lose uncommitted changes.


FIRST CHAPTER => 
1 jab bhi aap ek folder bnaate hai git ko kuchh nahi pata aapke folder
ke baare mein, isliye aap waha pe git ko initialize karte ho, ab git
ko permissions mili hai to git aapke folder ko pehchaanta hai, to ab
kyuki git kaam kar skta hai is folder per ab ham yaha par untracked,
tracked, modified, staged, and saved checkpoints create kar skte hai



------------------------------------------------------------------------------------------------------------------


GIT BRANCHING =>
 - CREATE BRANCH => git branch anyname , ex => git branch feature/footer
 - to see branch => git branch,
 - to switch branch => git switch filename  , ex => git branch feature/footer 
commit is importent 


HOW TO MERGE ? 
First we should be in main branch. Then use this command : git merge fileYouWantToMerge 
example => git merge feature/navbaar

HANDLING CONFLICT DURING MERGING=>
  -MERGING TECHNIQUES => ff merging
