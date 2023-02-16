# dev-env-standards

## Drupal Spefific Pre-commit hooks

Pre-commit hooks run various code formatters and linters. Some (black, prettier)
will automatically reformat your code.

These pre-commit settings were sourced from this article: https://www.cmsdrupal.com/blog/git-pre-commit-hook-how-commit-yourself-committing-clean-drupal-code-only

If you're using Visual Studio code
with the recommended extensions, the pre-commit hook formatting should match
editor output.

1. Install [pre-commit](https://pre-commit.com/#install) :
   `brew install pre-commit` (OS X) or `pip install pre-commit` (elsewhere).
2. Run the command `composer require drupal/coder dealerdirect/phpcodesniffer-composer-installer`
3. Add the file named `pre-commit` to the `./.git/hooks/` directory of your repository
4. Set up the pre-commit and commit message git hooks in the local repository:
   `pre-commit install --hook-type pre-commit --hook-type commit-msg`.
