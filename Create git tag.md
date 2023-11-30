    git checkout master
    git merge --no-ff <release_branch>
    git push origin master
    git tag -a <release_name>
    git push origin --tag <release_name>

verify if the merge was correclty done and tag is created in remote
do the steps below for the hotfix and the release branch

    git branch -d <release_branch> (delete local release branch)
    git push origin --delete <release_branch> (delete remote release branch)