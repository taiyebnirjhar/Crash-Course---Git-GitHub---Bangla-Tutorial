<link rel="stylesheet" type="text/css" href="style.css">

# [Crash Course - সহজ বাংলায় Git & GitHub - Bangla ( বাংলা ) Tutorial by Learn with Sumit](https://youtu.be/oe21Nlq8GS4)

### Fundamental Theory

Local

- working directory => Stage => local repository

For example:

1. git add . ( working directory => Stage )

2. git commit -m 'setup' ( Stage => local repository )

Remote

- local repository => remote

For example:

1. git push ( local repository => remote )

---

### Install git in Linux machine

1. Open a terminal window on your Linux machine.
2. Update the package list using the command:

```bash
sudo apt-get update -y
```

3. Once the package list is updated, install Git using the command:

```bash
sudo apt-get install git
```

4. After Git is installed, verify the installation by running the following command to check the Git version:

```bash
git --version
```

5. Now that Git is installed, it's a good idea to set your username and email address in Git. This information is used to identify who made changes to a repository.

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

---

### Play with git

#### 🔥 Initializing new git repository

```bash
git init
```

💡 Running "git init" in a directory creates a ".git" subdirectory with files for Git to manage the repository.

💡 ".git" that contains all of the necessary files for Git to manage the repository. These files include : `config`, `description`, `HEAD`, `index`, `hooks`

💁‍♂️ Deleting '.git' removes the repository's history and configuration

#### 🔥 Clone a git repository

```bash
git clone targeted-url
```

#### 🔥 Check current state / status

```bash
git status
```

#### 🔥 Staging / Adding changes to the staging area

1. Staging all file

```bash
git add -A
```

or

```bash
git add --all
```

2. Staging all files of current folder

```bash
git add .
```

3. Staging all changes except deleted files or risky changes in Git

```bash
git add *
```

4. Staging specific file

```bash
git add filename
```

or if the file is inside a children folder

```bash
git add foldername filename
```

#### 🔥 Commit

```bash
git commit -m 'your commit text'
```

#### 🔥 Reset / Unstage changes

1. "git reset" without any arguments

```bash
git reset
```

💡 Use 'git reset' without any arguments to quickly unstage all changes

2. We can also use "git reset" to unstage specific files or specific commits,

for specific file:

```bash
git reset HEAD file.txt
```

for specific commit:

```bash
git reset HEAD~1
```

💡 Here '1' referes to go back one commit.

for last commit

```bash
git reset HEAD~
```

💡 without the number it automatically refers to '1' / last commit

3. 'git reset' only resets staging. if we delete a file and we want reset the delete action & staging:

```bash
git reset --hard
```

#### 🔥 Remove

```bash
git rm filename
```

💡 remove + stage

#### 🚨 Branch

1. check available branch:

```bash
git branch
```

2. create new branch:

```bash
git branch new-branch-name
```

3. move to another branch

```bash
git checkout new-branch-name
```

#### 🚨 Merge

1. marging current branch with another branch. for example we are in 'checkone' branch and now we are trying to merge this with main branch

```bash
git merge main -m 'merging  checkone with main'
```

💡 Now checkone branch is upto date but main branch have no idea whats happening on other branches thats why we need to merge main branch with checkone

```bash
git checkout main
git merge checkone -m 'merging  main with checkone'
```

#### 🚨🚨 Merge Conflict

1. First, run `git status` to see which files have conflicts.
2. Open the conflicting file(s) in a code editor to view the merge conflicts. You will see sections of the code that have been marked with conflict markers such as <<<<<<< HEAD, =======, and >>>>>>>.
3. Edit the conflicting code to resolve the conflicts. You may need to consult with the other contributors to determine the appropriate changes.
4. After making the changes, stage the modified file(s) using git add.
5. Commit the changes using git commit.

#### ⚠️ Push

```bash
git push origin branchname
```

#### ⚠️ Fetch

```bash
git fetch
```

💡 `git fetch` downloads changes from a remote repository to your local repository, but does not merge those changes with your current branch. This command is useful for keeping your local repository up-to-date with changes made by other team members, without affecting your own work.

**To merge with the remote repository we need to merge manually**

```bash
git merge
```

#### ⚠️ Pull

```bash
git pull
```

💡 git Fetch + git merge
