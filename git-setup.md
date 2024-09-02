# Setting up git

1. Make a directory that will contain your local repository.

2. If setting up for the first time:
   - $ git config --global user.name "Your Name"
   - $ git config --global user.email "discombobulatedpancake@proton.me"
   - On macOS and Linux: $ git config --global core.autocrlf input
   - git config --global core.editor "kate"
   = git config --global init.defaultBranch main
3. cd into directory where you want the repository
4. $ git init

That's it for setting up a local repository for the first time.
After doing git-config you just need to git init.


5. Add a file to the directory that you want to track.
6. $ git add filename
7. $ git commit -m "message"
8. $ git status

## Linking to remote repository and pushing a remote copy

1. Create or login to github account.
2. Create new repository
3. Select ssh and copy the url
4. $ git remote add git@github.com:username/repository_name.git

If you haven't set up a ssh key pair for the machine you are on:

1. ssh-keygen -t ed25519 -C "username.domain.edu"
2. passphrase not necessary unless using shared computer
3. On github copy the ssh key in ~/.ssh/id_ed25519.pub to SSH keys from Settings
4. $ ssh -T git@github.com

5. $git push origin main
