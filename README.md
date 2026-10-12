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
