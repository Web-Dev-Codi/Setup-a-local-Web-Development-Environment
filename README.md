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

Change the name of the master branch to main (Very Important)

```bash
git config --global init.defaultBranch main
```

Enter in terminal to see the config

```bash
git config --list
```

The terminal should look something like this

```bash
git config --list
user.name=Your Github User Name Here
user.email=your@email.com
init.defaultbranch=main
```

# Generating an SSH key

Remain in the terminal and enter these commands

```bash
ssh-keygen -t ed25519 -C yourgithub@email.com
```

Hit Enter until the process is done

In the terminal open the file id_ed25519.pub inside the .ssh directory within your Home directory with the following command.

```bash
cat id_ed25519.pub
```

and copy paste the code to your github account by adding the ssh key the link here.

```url
https://github.com/settings/keys
```

Click New ssh key button
![alt text](sshbutton.png)
Fill out the required fields and click the add ssh key button
![alt text](newsshsubmit.png)

Once the ssh key is added, when you try to push/create a repository a popup with ask to add your system to github fully type yes.

Enjoy being connected to github via ssh
