# Commit message format

We rely on [**semantic-release**](https://github.com/semantic-release/semantic-release) for automated version management and package publishing, which uses the commit messages to determine the type of changes in the codebase. Following formalized conventions for commit messages, **semantic-release** automatically determines the next semantic version number, generates a changelog and publishes the release.

Engineers must follow the [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/).

## List of types we use:

- **build**: Changes that affect the build system or external dependencies (i.e. `package.json`, `netlify.toml`).
- **ci**: Changes to our CI configuration files and scripts (i.e. `.github/dependabot.yml`).
- **docs**: Documentation only changes.
- **feat**: A new feature.
- **fix**: A bug fix.
- **perf**: A code change that improves performance.
- **refactor**: A code change that neither fixes a bug nor adds a feature.
- **revert**: Undo changes from a previous commit.
- **static**: Changes to static asset types (i.e. images, PDFs, etc.)
- **test**: Adding missing tests, correcting existing tests, or running a test.
