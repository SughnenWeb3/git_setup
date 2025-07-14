1. What is Version control?
 Version control is a is a system that tracks and also manages changes to code or documents over time

2. What is version control used for ?
 It is basically used to mange and track files

3. What is git
 It is a free version control system

4. What is Github
 It is a platform that allows developers to create, store and manage their code

5. What is the difference between Git and github

Git is a version control system while Github is a platform that hosts repositories

6. Comprehensive steps on setting up a github account

The following steps apply in creating a github account for an abbsolute beginner.

Create a GitHub Account

Go to https://github.com/ and sign up for a free account.
Use a strong, unique password and verify your email address.
Install Git on Mac using Homebrew

Open the Terminal on your Mac.
Install Homebrew if you don’t already have it by running:
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
Install Git using Homebrew:
brew install git
Verify the installation:
git --version
Configure Git

Set your username:
git config --global user.name "Your Name"
Set your email address (use the same email as your GitHub account):
git config --global user.email "your-email@example.com"
Authenticate Git with GitHub

Generate an SSH key:
ssh-keygen -t ed25519 -C "your-email@example.com"
Press Enter to accept the default file location and set a passphrase if desired.
Add the SSH key to the SSH agent:
eval "$(ssh-agent -s)"
ssh-add --apple-use-keychain ~/.ssh/id_ed25519
Copy the SSH key to your clipboard:
pbcopy < ~/.ssh/id_ed25519.pub
Add the SSH key to your GitHub account:
Go to GitHub SSH settings.
Click New SSH key, paste the key, and save.
Create a Repository on GitHub

On GitHub, click the + icon in the top-right corner and select New repository.
Name your repository, add an optional description, and click Create repository.
Clone the Repository Locally

Copy the SSH URL of your repository from GitHub.
In the Terminal, clone the repository:
git clone git@github.com:your-username/your-repository.git
Add Files and Push Changes

Navigate to the repository folder:
cd your-repository
Create a file (e.g., README.md):
echo "This is my first repository" >> README.md
Stage and commit the file:
git add README.md
git commit -m "Add README"
Push the changes to GitHub:
git push -u origin main



