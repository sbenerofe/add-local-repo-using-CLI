# add-local-repo-using-CLI

Adding a local repository to GitHub with GitHub CLI
In the command line, navigate to the root directory of your project.

Initialize the local directory as a Git repository.

git init -b main
Stage and commit all the files in your project

git add . && git commit -m "initial commit"
To create a repository for your project on GitHub, use the gh repo create subcommand. When prompted, select Push an existing local repository to GitHub and enter the desired name for your repository. If you want your project to belong to an organization instead of your user account, specify the organization name and project name with organization-name/project-name.

Follow the interactive prompts. To add the remote and push the repository, confirm yes when asked to add the remote and push the commits to the current branch.

Alternatively, to skip all the prompts, supply the path to the repository with the --source flag and pass a visibility flag (--public, --private, or --internal). For example, gh repo create --source=. --public. Specify a remote with the --remote flag. To push your commits, pass the --push flag. For more information about possible arguments, see the GitHub CLI manual.
