# Daily GitHub activity

This repository records one UTC date in `activity.log` each day. The
`Daily activity` GitHub Actions workflow runs daily at 09:00 UTC and commits
the entry; it can also be started manually from the repository's **Actions**
tab.

## Set up

1. Create a GitHub repository and push these files to its default branch.
2. In the repository, open **Settings → Actions → General** and allow
   workflows read and write access to repository contents.
3. Open the **Actions** tab and enable workflows if GitHub prompts you.

The scheduled run uses GitHub's built-in `GITHUB_TOKEN`; no personal access
token or secret is required. Entries are appended to the log, and rerunning
the workflow on the same UTC date won't create a duplicate commit.
