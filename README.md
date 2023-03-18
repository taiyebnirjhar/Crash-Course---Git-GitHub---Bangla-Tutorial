# Crash Course - সহজ বাংলায় Git & GitHub - Bangla ( বাংলা ) Tutorial by Learn with Sumit

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
