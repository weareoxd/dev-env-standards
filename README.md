# dev-env-standards

## Pre-commit hooks

Pre-commit hooks run various code formatters and linters. Some (black, prettier) 
will automatically reformat your code. 

If you're using Visual Studio code 
with the recommended extensions, the pre-commit hook formatting should match 
editor output.

1. Install [pre-commit](https://pre-commit.com/#install) :
   `brew install pre-commit` (OS X) or `pip install pre-commit` (elsewhere).
2. Add the file named `.pre-commit-config.yaml` to the root of your repository 
   and list the pre-commit hook checks that you want to run 
   (see example hooks in `.pre-commit-config.<name>.yaml` split by technology).
3. (Optional) If you use [Gitlint hook](https://github.com/jorisroovers/gitlint), 
   add `.gitlint` file to set custom git commit linting rules (see example).
4. Set up the pre-commit and commit message git hooks in the local repository: 
   `pre-commit install --hook-type pre-commit --hook-type commit-msg`.
