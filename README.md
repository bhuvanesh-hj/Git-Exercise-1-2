# Git Exercise Report 1 and 2

## Exercise 1

### Main Task:

1. **Creating a New Repository:**
   - Created a new directory `exercise1` and initialized a Git repository using `git init`.
   - Verified the presence of the `.git` directory.

2. **Creating README File:**
   - Created a `README.md` file in the repository.

3. **Adding and Committing README:**
   - Checked status using `git status`; `README.md` was listed as untracked.
   - Added `README.md` to the staging area with `git add README.md`.
   - Committed changes using `git commit -m "Added README.md"`.

4. **Creating src Directory and Files:**
   - Created a `src` directory and added files `file1.txt` and `file2.txt`.

5. **Adding Files to Staging Area:**
   - Used `git add src` to stage changes from the `src` directory.
   - Checked status to verify both files (`file1.txt`, `file2.txt`) were staged.
   - Committed changes with `git commit -m "Added files in src directory"`.

6. **Viewing and Staging Changes:**
   - Made a change to `file1.txt` and used `git diff` to view the changes.
   - Added `file1.txt` to the staging area using `git add file1.txt`.
   - Noticed `git diff` showed no changes after adding to staging.

7. **Managing Staged and Unstaged Changes:**
   - Made another change to `file1.txt` without committing.
   - Checked status to see staged and unstaged changes.
   - Used `git add file1.txt` to stage the latest changes.
   - Committed changes with appropriate message.

8. **Viewing Commit History:**
   - Used `git log` to view all commits made so far.
   - Each commit was displayed with a commit identifier.

9. **Using Short Commit Identifiers:**
   - Used `git show <commit_id>` to view details of an individual commit.
   - Found that a minimum of 7 characters of the commit identifier could be used.

### Stretch Task:

1. **Using Git rm Command:**
   - Used `git rm <filename>` to remove a file and committed the deletion.

2. **Deleting a File without Git:**
   - Deleted another file using OS-specific command (`rm` on Linux).
   - Compared status to `git rm` command; noted differences.

3. **Using Git mv Command:**
   - Renamed `README.md` to `README.txt` using `git mv`.
   - Committed the rename change.

4. **Renaming Without Git:**
   - Renamed `README.txt` to `README_v2.txt` using OS command.
   - Observed incorrect status; files appeared as deleted and untracked.
   - Used `git add` to resolve status and committed.

5. **Displaying Recent Commits:**
   - Used `git help log` to find `git log -n 3` for displaying recent commits.

6. **Using --stat Option:**
   - Reviewed slides for `--stat` option on `git diff`.
   - Confirmed it also worked with `git show` and `git log`.

7. **Viewing Diff Between Commits:**
   - Used `git diff <commit_id1>..<commit_id2>` to summarize changes between two commits.

## Exercise 2

### Main Task:

1. **Checking Branch Status:**
   - Ran `git status` to identify current branch (`master`).

2. **Creating and Switching Branches:**
   - Created a new branch `feature-branch` using `git branch feature-branch`.
   - Checked out the new branch with `git checkout feature-branch`.

3. **Making Commits in Branch:**
   - Made several commits in `feature-branch`, including file additions and edits.

4. **Viewing Commit History:**
   - Used `git log` to see recent commits in `feature-branch`.

5. **Switching Back to Master:**
   - Checked out `master` branch using `git checkout master`.
   - Observed original file contents and no commits from `feature-branch` in `git log`.

6. **Visualizing Branch History:**
   - Used `gitk` to visualize the linear commit history in `feature-branch`.

7. **Merging Branches:**
   - Merged `feature-branch` into `master` using `git merge feature-branch`.
   - Confirmed fast-forward merge in `git log` and `gitk`.

### Stretch Task:

1. **Handling Merge Conflicts:**
   - Created conflicting changes in the same lines between `master` and `feature-branch`.
   - Attempted merge resulted in conflict; edited files to resolve conflicts.
   - Added resolved files to staging area and committed the merge.

2. **Restoring Working Copy:**
   - Deleted all files except `.git` and restored using `git checkout`.

3. **Handling File Deletion Conflict:**
   - Explored scenario where one branch modified a file and another deleted it.
   - Investigated resolution strategies.

4. **Customizing Merge Commit Message:**
   - Referenced `git help merge` for specifying a custom message.

5. **Manual Merge Commit:**
   - Explored options for preventing Git from auto-committing merge commits.

