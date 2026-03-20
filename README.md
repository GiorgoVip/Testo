# Testo
Testing with git
-[ GIT COMMANDS ]-

git config <CONFIG> (<VALUE>)      #// git config user.name user.email etc. git config --local for current git proj only --global for all

# Session/Commit related (Staging area) #

git init                           #// Init a new git proj

git remote add origin [-t <branch>] <link.git>
git remote                         #// for all things outside ur current git proj

git branch [-M <branch>]

git add [--all]                    #// add files to current commit  #// add updates specific or all files, so if u have a file removed and you want to remove it from the staging area (session) rerun the same add command to update (remove in this case) the file or u can remove the file via git rm  #// things like *.txt are supported here
git rm [--all]                     #// remove files from stage/session
git mv <src> <dst>                 #// rename /move files

git commit -m <commitName>         #// finish current commit


# origin related #

git push -u origin main --force    #// push current commit to origin

git pull <link.git> main           #// update with online
