# Branch Naming

- `topic/issue-17-fix-login-bug` for all work intended to be merged (bug fixes, features, etc.)
- `release/v1.2.5` for releasing multiple branches together
- `test/experimenting-with-tailwind` for throw-away branches

## Topic branches

In most cases, all planned work will have a related GitHub Issue created. If one doesn't exist, please consider creating one if the context of the work is worth documenting for our history. Since we use GitHub project boards to manage our projects, it also helps provide visibility into our workload.

Issues should be referenced in the branch name: `topic/issue-17-fix-login-bug`.

In all other scenarios, please adhere to the format in the following example: `topic/investigate-cms-config-errors`.

## Release branches

Our goal is always to merge issue branches into our main branch, but sometimes new features or sprints will require us to merge multiple issue branches into a release branch before merging the release branch into the main branch.

This is to ensure all issue branches work well together before deploying them to production.

## Test branches

Sometimes devs need to test out some ideas that will never get merged. This is what test branches are for.

In the event that a test branch becomes a branch with mergeable code, follow these workflow steps:

1. If there is no existing issue created for this work, create a new one.
2. Rename your test branch to one that follows the `issue/*` pattern.
