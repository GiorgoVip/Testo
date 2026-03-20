# Testo
Testing with git
-[ GIT COMMANDS ]-

git config <CONFIG> (<VALUE>)      #// git config user.name user.email etc. git config --local for current git proj only --global for all

# Session/Commit related (Staging area) #

git init                           #// Init a new git proj

git remote add origin (-t <branch>) <link.git>
git remote                         #// for all things outside ur current git proj

git branch (-M <branch>)

git add (--all)                    #// add files to current commit  #// add updates specific or all files, so if u have a file removed and you want to remove it from the staging area (session) rerun the same add command to update (remove in this case) the file or u can remove the file via git rm  #// things like *.txt are supported here
git rm (--cached) (--all)          #// remove files from stage/session
git mv <src> <dst>                 #// rename /move files


#// put files or directories in .gitignore to ignore it, if you want to ignore a file that is already in session/stage then u need to remove it first with git rm --cached <file 'or' -r dir> #// * *.<ext> is supported
git ls-files #// to see the files in stage/session
git diff (--staged)                #// see differences

git commit -m <commitName>                         #// finish current commit
git log (--oneline) (--reverse)                    #// see the commits most recent from top ('q' to quit)
git show <id> (HEAD) (HEAD~n) (<HEAD>:<file>)      #// show the changes in the commit, <id> is gotten from the log or tree
git ls-tree (<HEAD>) (<id>)        #// show tree final
git restore (--staged) <file>      #// restore a file or discard changes
git restore --source=<HEAD 'or' id> <file>   #// restore a file to an older version
git clean                          #// ! clear out the stage/session

# origin related #

git push -u origin main --force    #// push current commit to origin

git pull <link.git> main           #// update with online
