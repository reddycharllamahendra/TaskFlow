# TaskFlow
Day 2 Git fetch and pull practice.
1. Discover remote changes:
git fetch origin
Downloaded remote information without integrating it.

3. Check branch status
git status -sb
Reported that your local branch was one commit behind.

5. Identify incoming commits
git log --oneline main..origin/main
Listed commits recorded remotely but missing locally.

6. Inspect the actual changes
git diff main..origin/main -- README.md
Showed the exact file differences before integration.

7. Integrate the changes
git pull
Updated your local branch and working files.

Branch: local vs remote
1. Local Branch
Definition: A local branch is a branch in your local Git repository that allows you to develop features, modify code, and create commits independently without immediately affecting other branches or the remote repository.

Example: feature-login
You can work on login functionality in this branch without immediately changing main.

2. Remote-Tracking Branch
Definition: A remote-tracking branch is a local reference that records the last known state of a branch in a remote repository, such as GitHub. Git updates this reference when you fetch changes from the remote repository.

Example: origin/main
It helps you compare your local work with the last known state of the remote main branch.