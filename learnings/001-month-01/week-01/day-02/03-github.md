# Push code to Github

## Step 1: Install git 
If you haven't already, you need to install git on your computer. You can download it from [git-scm.com](https://git-scm.com/).

## Step 2: Initialize a git repository
Navigate to your project folder in the terminal and run the following command to initialize a git repository:
```bash
git init
```

## Step 3: Add files to staging area
You can add all files in your project to the staging area using the following command:
```bash
git add .
```

## Step 4: Commit your changes
After adding the files to the staging area, you need to commit your changes with a message describing what you have done. Use the following command:
```bash
git commit -m "Initial commit with temperature converter project"
```

## Step 5: Create a new repository on GitHub
Go to [GitHub](https://github.com/) and create a new repository. Do not initialize it with a README, .gitignore, or license, as you already have a local repository.

## Step 6: Add remote repository
After creating the repository on GitHub, you will get a URL for your repository. You need to add this URL as a remote repository in your local git configuration. Use the following command, replacing `<your-repo-url>` with the URL of your GitHub repository:
```bash
git remote add origin <your-repo-url>
```

## Step 7: Push your code to GitHub
Finally, you can push your local commits to the remote repository on GitHub using the following command:
```bash
git push -u origin master
```

This will push your code to the master branch of your GitHub repository. You may be prompted to enter your GitHub username and password if you haven't set up SSH keys or a credential manager.

