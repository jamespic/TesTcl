
Script for replacing verision number in all files

Mac OS X/Free BSD

    find -E .. -regex '^.*\.(tcl|md)$' -exec sed -i '' 's/OLD_VERSION_NUMBER/NEW_VERSION_NUMBER/g' {} \;

Tagging a new release and pushing to origin

    git tag -a v1.0.7 -m 'Release 1.0.7' 
    git push --tags

Remove feature branches after merging

    git branch -d feature_branch
    git push origin --delete feature_branch 
