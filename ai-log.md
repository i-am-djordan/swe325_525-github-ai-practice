<<<<<<< Updated upstream
=======
# AI Log
# Date: 9/26/2026
# AI Assistant: Claude

## Entry 1: Git and GitHub Concepts

### Prompt

> Explain the difference between a repository, branch, commit, pull request, and issue.

### Response

#### Repository
A **repository** (repo) is the project itself: all of its files, folders, and the full history of every change made to them. On GitHub, a repo also holds the project's issues, pull requests, and settings. Everything else on this list lives inside a repository.

#### Commit
A **commit** is a saved snapshot of the repository at one point in time. Each commit records what changed, who made the change, when, and a message explaining why. Every commit has a unique ID (a SHA hash) and points to the commit before it, so together they form the project's history. You can go back to any commit at any time.

#### Branch
A **branch** is an independent line of development: a movable pointer to a series of commits. The default branch (usually `main`) holds the stable version of the project. Developers create new branches (e.g., `feature/login`) to work on changes without affecting `main`. New commits on a branch only move that branch forward.

#### Pull Request
A **pull request** (PR) is a request to merge the commits from one branch into another, usually from a feature branch into `main`. It gives teammates a place to review the changes, see the differences (the "diff"), leave comments, run automated checks, and approve the work before it is merged. A PR is a GitHub collaboration feature, not part of Git itself.

#### Issue
An **issue** is a way to track work or discussion: a bug report, a feature request, a task, or a question. Issues contain no code. They describe *what* needs to be done. A PR can reference an issue (e.g., "Closes #12") so the issue closes automatically when the PR is merged.

#### How They Fit Together

| Concept | What it is | Contains code? |
|---|---|---|
| Repository | The whole project and its history | Yes |
| Commit | One snapshot of changes | Yes |
| Branch | A line of commits developed separately | Yes |
| Pull Request | A proposal to merge one branch into another, with review | Refers to commits |
| Issue | A tracked task, bug, or idea | No |

**Typical workflow:** An **issue** describes a bug → a developer creates a **branch** in the **repository** → makes one or more **commits** that fix it → opens a **pull request** to merge the branch into `main` → after review, the PR is merged and the issue is closed.

## Entry 2: README Review

### Prompt

> Review README.md for clarity and suggest revisions.

### Response Summary

The AI reviewed `README.md` and made seven suggestions:

1. Remove the second H1 heading. Line 3 was a full sentence written as a heading, so turn it into normal paragraph text under a single title.
2. Fix the typo "reject suggestions" → "rejected suggestions".
3. Rename "Scope" to "Lab Requirements" and turn the list into a checklist (`- [ ]`).
4. Replace the vague "demonstrates AI usage within GitHub" with a specific statement that AI use is recorded in `ai-log.md`.
5. Add a "Contents" section listing the repository's files.
6. Change the bare issue URL to a labeled link (`[Issue #1](...)`).
7. Replace the "Student - Destiny Jordan" heading with an "Author" section that includes the course name.

### Decision

| # | Suggestion | Decision | Notes |
|---|---|---|---|
| 1 | Single H1 title; heading sentence becomes paragraph | Accepted | |
| 2 | Fix "reject" → "rejected" | Accepted | |
| 3 | "Scope" → "Lab Requirements" checklist | Accepted | |
| 4 | Clarify how AI use is documented | Accepted | |
| 5 | Add "Contents" section | Accepted | |
| 6 | Labeled issue link | Accepted | |
| 7 | "Author" section with course name | Accepted | |

All suggestions were accepted as written, and the revised README was applied.

## Entry 3: Pull Request Description Checklist

### Prompt

> Suggest a checklist for a complete pull-request description.

### Response Summary

The AI suggested seven sections for a complete PR description. The first three match the lab requirements (summary, issue link, evidence).

1. **Summary**: a clear title plus one or two sentences on what changed and why.
2. **Related issue**: link the issue with a closing keyword (e.g., `Closes #1`) so it closes automatically on merge.
3. **Evidence**: screenshots, before/after comparisons, or links to commits and files showing the requirements are met.
4. **Changes made**: a bullet list of specific changes, plus anything intentionally left out.
5. **Testing or verification**: how the change was checked (e.g., previewing rendered Markdown, confirming links work).
6. **AI use**: whether AI tools were used, with a pointer to `ai-log.md`.
7. **Review readiness**: correct base branch, no merge conflicts, reviewers assigned if required.

### Decision

| # | Suggestion | Decision | Notes |
|---|---|---|---|
| 1 | Summary | Rejected | Not implemented |
| 2 | Related issue with closing keyword | Rejected | Not implemented |
| 3 | Evidence | Rejected | Not implemented |
| 4 | Changes made | Rejected | Not implemented |
| 5 | Testing or verification | Rejected | Not implemented |
| 6 | AI use | Rejected | Not implemented |
| 7 | Review readiness | Rejected | Not implemented |

All suggestions were rejected. The checklist and template were not used for this lab's pull request.

1. Which GitHub action or object was most useful to you, and why?
    The pull request was the most useful. It made me actually review the work and changes that I made to ensure that it actually works for the project.
2. Which AI suggestion did you accept, and what made it useful?
    I accepted the AI's rewire of README.md. It fixed a heading sturcture issue that I didn't even notice. It caught a typo and added a scioe section. It was useful because it aligned the file with what the lab actually required.
3. Which AI suggestion did you revise or reject, and why?
    I rejected the AI's suggested pull-request checklist template. I hadn't made the pull request at the time so there wasn't a need for it yet.
4. What did you verify yourself instead of trusting the AI?
    I verified the actual commit hashes and URLs myself by checking GitHub directly. I also confirmed the branch name and merge status directly on GitHub.
5. What would you change in your GitHub workflow next time?
    I'd fill in workflow-notes.md incrementally as I created each commit and the PR, rather than leaving several fields as placeholders and coming back to fill them in at the end.
>>>>>>> Stashed changes
