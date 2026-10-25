# Contributing

This repository is a sandbox for practicing small, verifiable changes through pull requests.

## Make a change

1. Clone the repository and enter its directory:

   ```sh
   git clone https://github.com/eloooong/codex_test.git
   cd codex_test
   ```

2. Start a branch from the latest `main`:

   ```sh
   git switch main
   git pull --ff-only
   git switch -c describe-your-change
   ```

3. Make one focused improvement. Review the diff and check whitespace:

   ```sh
   git diff
   git diff --check
   ```

4. Stage only the files you intend to include, review the staged diff, and commit:

   ```sh
   git add path/to/changed-file
   git diff --cached
   git diff --cached --check
   git commit -m "Describe the improvement"
   git push -u origin describe-your-change
   ```

5. Open a pull request targeting `main`. Explain the problem, the change, and how you validated it. Include `Closes #ISSUE_NUMBER` when the change resolves an existing issue.

6. Check the final diff and any checks shown on the pull request before merging. For code changes, run the relevant tests; this sandbox currently has no automated test suite.

## Keep the history useful

- Keep unrelated changes in separate pull requests.
- Credit coauthors only when they actually contributed to a commit.
- Leave operating system metadata and editor backup files untracked.
