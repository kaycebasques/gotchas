# git

## get a branch from a remote repo

    git fetch git@github.com:theirusername/reponame.git theirbranch:ournameforbranch

https://stackoverflow.com/a/42716331/1669860

## rename a remote

    git remote rename previous new

## delete all local branches except master

    git branch | grep -v "master" | xargs git branch -D 

## delete branch locally and remotely

    git push --delete <remote_name> <branch_name>
    git branch -d <branch_name>
