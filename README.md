# Setting up your git credentials

In your terminal enter these commands without quotes

Enter your Github user name

```bash
git config --global user.name "Your Github User Name Here"
```

Enter the email you used to signup for GitHub

```bash
git config --global user.email "your@email.com"
```

Change the name of the mastere branch to main (Very Important)

```bash
git config --global init.defaultBranch main
```

# Generating an SSH key

```bash
ssh-keygen -t ed25519 -C yourgithub@email.com
```

Hit Enter until the process is done

Open the file id_ed25519.pub inside your .ssh directory and copy paste the code to your github account by adding the ssh key here.

```url
https://github.com/settings/keys
```

Once the ssh key is added, when you try to push/create a repository a popup with ask to add your system to github fully type yes.

Enjoy being connected to github via ssh
