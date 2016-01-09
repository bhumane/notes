GIT CHEAT SHEET

The purpose of this sheet is to teach me the basic git commands and keep track of usefull commands and shortcuts.

# Create a new git repo
1- You can do this from the git UI by clicking on create new repo (+ sign on top right, next to your profile) and give it a name and description and keep it public.

2- setup ssh keys between github and your machine.
    - ssh-keygen
    - cat know_hosts
    - In the top right corner of any page, click your profile photo, then click Settings.
    - In the user settings sidebar, click SSH keys.
    - Click Add SSH key.
    - In the Title field, add a descriptive label for the new key. For example, if you're using a personal Mac, you might call this key "Personal MacBook Air".
    - Paste your key into the "Key" field.
    - Click Add key.
    - Confirm the action by entering your GitHub password.

3- git clone git@github.com:bhumane/notes.git

4- always create .md (markdown files)

5- [ Sat Jan- 9-2016  14:03:12 ] git:(master) 1M 1A  bharati@ubuntu: ~/notes
note from the above lime it means that I'm on the master branch and I've 1 modified file (1M) and I added 1 new file (1A)

6- optionally you cab type gss or git status
Eg-
branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
    (use "git checkout -- <file>..." to discard changes in working directory)

            modified:   tmux_cheat_sheet.md

            Untracked files:
              (use "git add <file>..." to include in what will be committed)

                      git_cheat_sheet.md

                      no changes added to commit (use "git add" and/or "git commit -a")

7- You need to add the files you can give the filename or use . (which means add all files)
git add . or shortcut gaa

8- then you need to commit the files
git commit -m "first check in"

9- Finally you push the files to github repo
git push origin master

10- How do you know what is orgin and what is master. 
cat .git/config

Output of the above command:
[core]
        repositoryformatversion = 0
                filemode = true
                        bare = false
                                logallrefupdates = true
                                [remote "origin"]
                                        url = git@github.com:bhumane/notes.git
                                                fetch = +refs/heads/*:refs/remotes/origin/*
                                                                     [branch "master"]
                                                                             remote = origin
                                                                                     merge = refs/heads/master


11- what are the various git shortcuts
alias | grep git
