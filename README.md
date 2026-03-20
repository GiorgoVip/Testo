# Testo
Testing with git
-[ GIT COMMANDS ]-

git config <CONFIG> (<VALUE>)      #// git config user.name user.email etc. git config --local for current git proj only

# Session/Commit related #

git init                           #// Init a new git proj

git remote add origin [-t <branch>] <link.git>
git remote                         #// for all things outside ur current git proj

git branch [-M <branch>]

git add [--all]                    #// add files to current commit

git commit -m <commitName>         #// finish current commit


# origin related #

git push -u origin main --force    #// push current commit to origin

git pull <link.git> main           #// update with online
