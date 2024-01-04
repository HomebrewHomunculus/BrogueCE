# Brogue Lite -specific development notes

## How to merge upstream changes from BrogueCE mainline

Create a new branch.

Check which commit matches the release, e.g. https://github.com/tmewett/BrogueCE/releases/tag/v1.13 => https://github.com/tmewett/BrogueCE/commit/dfd321ed82b104ed141323baefc6fef1c7b60315
Merge that commit (since we're not able to use tags as merge targets).

```
git checkout -b merge-upstream-v1.13
git fetch upstream 
git merge dfd321ed82b104ed141323baefc6fef1c7b60315
```

Then fix conflicts.

Then push to origin, create a PR, and so on.