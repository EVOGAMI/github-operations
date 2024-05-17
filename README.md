# GitHub Operations

All of our work will be stored on GitHub, so it is important to understand how to use it. 

## 1. Convention

### 1.1 Issues

- Each issue should be a single logical task. 

  For example, fixing a typo, adding a new feature, or refactoring a class.

- Each issue should have a descriptive title.

    The title should be in the format `<short description>`. For example, `Fix typo`.

- Each issue should have a descriptive body.

    The body should describe the task to be completed.

- Each issue should be assigned to at least one team member.

- Each issue should be labeled with at least one label.

    I will set up labels for the repository.

- Each issue should be linked to at least one milestone.

    I will set up milestones for the repository.

- Each issue should be linked to at least one project.

    In our case, the project will be EVOGAMI.

### 1.2. Branches

- `main`: The main branch of the repository. 

  This branch should always be stable -- buildable and testable.

- issue branches: Branches created for specific issues. 

  These branches should be created from `main` and merged back into `main` when the issue is resolved.

  The branch name should be `issue-<issue number>-<short description>`. For example, `issue-1-fix-typo`.

- local branches: Branches created for local testing and development.

  These branches should stay local and should not be pushed to the remote repository.

  The branch name should be `<name>-<short description>`. For example, `lance-fix-typo`.

- Always merge the latest changes from `main` into your branch before creating a pull request.

    This will help to avoid merge conflicts.

    ```sh
    git fetch origin
    git merge origin/main
    ```

### 1.3. Commits

- Each commit should be a single logical change. 

  For example, fixing a typo, adding a new feature, or refactoring a class.

- Each commit should have a descriptive commit message.
    
  The commit message should be in the format `<type> <description>`. For example, `Fix typo in README`.

    The commit message should be in the present tense. For example, `Fix typo in README` instead of `Fixed typo in README`.

    The commit message should be in the imperative mood. For example, `Fix typo in README` instead of `Fixing typo in README`.

    The commit message should be less than 50 characters. For example, `Fix typo in README` instead of `Fixed a typo in README.md and add a new line to the file which was missing`.

### 1.4. Pull Requests

- Each pull request should resolve a single issue.

    If a pull request resolves multiple issues, it should be split into multiple pull requests.

- Each pull request should have a descriptive title.

    The title should be in the format `Resolve <issue number> - <short description>`. For example, `Resolve #1 - Fix typo`.

- Each pull request should have a descriptive body.

    The body should describe the changes made in the pull request.

    I will set up a template for the pull request body.

- Each pull request should be reviewed by at least one other team member.

    I will configure the repository to require at least one review before a pull request can be merged.

    If you are reviewing a pull request, you should leave comments on the pull request.

    - For art, assign at least one art student to review the pull request.

    - For cs, assign at least one CS student to review the pull request.

    - For music, always assign Lyndon. 
    
        *To Lyndon: you can review the pull request yourself as you see fit.*

- When reviewing a pull request, you should check the following:

    - The changes are correct and complete.

    - The changes are consistent with the issue description.

    - The changes are consistent with the pull request description.

    - The changes are consistent with the conventions.

    - The changes do not introduce any new issues.

    - The changes do not break any existing functionality.

- When merging a pull request, you should always

    - Check for and resolve any merge conflicts.

    - Use the "Squash and merge" option.

        You can leave the commit message as is or update it as needed.