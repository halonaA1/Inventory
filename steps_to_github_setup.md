## Steps to setup a GitHub repository for the first time

- First create your GitHub account if you haven't already.
- Create a new repository and name it. Provide a brief description (optional)
- Add a new ssh key to your github account from the computer you are using. To do this, first create a keypair from your terminal. Assuming you are using a bash terminal, enter the command `ssh-keygen`. Navigate to the `~/.ssh/` directory and enter the command `cat id_(name_of_file).pub`. This will display the public key of the keypair generated. Copy it. Go to your GitHub dashboard and click your account icon on the rop right side of your screen then navigate to `Your Organizations`. Go to `SSH and GPG Keys` and select `New SSH key`. Paste the content you had copied from your terminal and create the ssh key.
- On your pc, open the project folder and initialise it as a Git repository by entering the command `git init` in your terminal.
- Rename the branch to `main` using the command `git branch -M main` (Optional, just a common industsry standard to have the primary branch as main).
- Connect your local repo to your upstream repo (GitHub) using the command `git remote add origin main git@github.com:GITHUB_USERNAME/GIHUB_REPO_NAME.git`. (Steps are outlined on the screen after creating your GitHub repo).
- Create a file adnd stage it using the command `git add FILE_NAME`.
- Create a commit from the staged files: `git commit -m "COMMIT MESSAGE"
- Push the commit to the upstream repo: `git push`. When pushing for the first time, use the command `git push --set-upstream origin NAME_OF_BRANCH` or `git push -u origin`.