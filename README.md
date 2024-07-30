# ITI_PHP
#Tell me how to remove them locally and remotely
1. Remove Local Branches
# Ensure you are on the main branch
git checkout main

# Delete the local dev branch
git branch -d dev

# Delete the local test branch
git branch -d test

2. Remove Remote Branches
-# Delete the remote dev branch
git push origin --delete dev

# Delete the remote test branch
git push origin --delete test

--------------------------------------
# Tell me how to checkout another branch without commit changes 
# Save your uncommitted changes
git stash

# Switch to another branch
git checkout branch_name

# Optionally, apply the stashed changes
git stash pop

----------------------------------------------------------
# Tell me how to list tags.
# List all tags
git tag

# List tags with detailed information
git show-ref --tags

# List tags with descriptions
git tag -n

# List tags matching a pattern (e.g., tags starting with 'v1.')
git tag -l 'v1.*'

---------------------------------------------------------------
# Tell me how to delete tag locally and remotely.

# List all tags to confirm the tag you want to delete
git tag

# Delete the local tag
git tag -d tag_name

# Delete the remote tag
git push origin --delete tag_name

----------------------------------------------------------------

