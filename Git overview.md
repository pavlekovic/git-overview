# Git

## What is Git?
Git is distributed version control system (VCS) that helps developers track changes in their code and collaborate on projects more efficientlu.

## Key Features of Git:
1. **Version Tracking**: Keeps a history of all changes made to files in a project.
2. **Branching and Merging**: Developers can work on separate branches (e.g., for new features or bug fixes) and merge their work into the main branch when ready.
3. **Distributed System**: Every user has a full copy of the project repository, including its history, on their local machine.
4. **Collaboration**: Makes it easy for teams to work together and track contributions.
5. **Efficiency**: Handles large projects and files quickly.

Git comes with a command-line user interface (Git bash), but GUI version is also available (Github Desktop).

### Other features include
- Repositories: a folder or directory controlled by Git.
- Projects: useful in planing SCRUM/AGILE projects.

## Syncronizing changes
### If the changes are made locally:
- Add the changed files to the staging area with `git add`
- Commit the changes to the local repo with `git commit -m <message>`
- Push the changes to the remote repo with `git push`

### If the changes are made remotely:
- Pull the new version of the files with `git pull`

The three stages of Git can be seen in the diagram below:

![Three stages of Git](https://miro.medium.com/v2/resize:fit:800/1*tl3B9CRamhIw54usIfXubw.png)

## Common Commands:
- `git init`: Initialize a new Git repository.
- `git clone`: Copy an existing repository to your local machine.
- `git add`: Stage changes for the next commit.
- `git commit`: Save a snapshot of your changes to the repository.
- `git push`: Upload your changes to a remote repository (e.g., GitHub).
- `git pull`: Download and integrate changes from a remote repository.
- `git status`: Check the status of your working directory.
- `git diff`: Check the differences between working files and commits.
- `git log`: A comprehensive list (log) of everything that has happened.

## Collaboration
**Single branch project** is fine for a solo developer, but for a team of developers, **multiple branch project** is used.
Git branches are used to isolate work. Each developer can create a branch to work on a specific feature, bug fix, or experiment without interfering with others. To create and switch to a new branch `git checkout -b <branch name>` command is used. Making and commiting changes, pushing changes to remote, and pull (merge) requests are the same as in solo work.

When a feature or fix is ready to be integrated, developers open a pull request (on GitHub) or merge request (on GitLab). This process involves:
- Reviewing the changes. 
- Discussing improvements. 
- Resolving conflicts (if any).

Once approved, the branch is merged into the main branch (e.g., main or master).

### When merging, if:
- The branch is only main or dev branch, then:
  - Create a pull request
  - Assign reviewers
  - Merge once all changes have been approved
- The branch is both behind and ahead of main or dev branch, then:
  - Pull request to merge latest dev into the branch
  - Another pull to merge the other way
  - Approval process as before

Any conflicts are usually resolved locally. To reduce conflicts, it is crucial to:
- Have good communication.
- Let everyone in teh team know which files you are working on.
- Have a standard process which everyone follows.