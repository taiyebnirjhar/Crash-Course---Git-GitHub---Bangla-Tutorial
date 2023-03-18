<link rel="stylesheet" type="text/css" href="style.css">

# [Crash Course - সহজ বাংলায় Git & GitHub - Bangla ( বাংলা ) Tutorial by Learn with Sumit](https://youtu.be/oe21Nlq8GS4)

### Fundamental Theory

<br>

Local

- working directory => Stage => local repository

For example: <br>

1. git add . ( working directory => Stage )

2. git commit -m 'setup' ( Stage => local repository )

Remote

- local repository => remote

For example: <br>

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

<br>

###### 🔥 Initializing new git repository

```bash
git init
```

💡 Running "git init" in a directory creates a ".git" subdirectory with files for Git to manage the repository.

💡 ".git" that contains all of the necessary files for Git to manage the repository. These files include : `config`, `description`, `HEAD`, `index`, `hooks`

💁‍♂️ Deleting '.git' removes the repository's history and configuration

<br>

###### 🔥 Clone a git repository

```bash
git clone 'targeted-url'
```

<br>

###### 🔥 Clone a git repository

```bash
git clone 'targeted-url'
```
