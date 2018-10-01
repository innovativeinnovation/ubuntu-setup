# GitHub

[GitHub](https://github.com/) is a web-based hosting service for version
control using Git.

### Connecting to GitHub with SSH

The instructions below are referenced from
[the official documentation](https://help.github.com/articles/connecting-to-github-with-ssh/).

Using the SSH protocol, you can connect and authenticate to remote servers
and services. With SSH keys, you can connect to GitHub without supplying
your username or password at each visit.

Check for existing SSH keys:

```bash
ls -al ~/.ssh
```

Generate a new SSH key:

```bash
ssh-keygen -t rsa -b 4096 -C "you@example.com"
```

Add your SSH key to the ssh-agent:

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

Add the SSH key to your GitHub account:

```bash
sudo apt install xclip
xclip -sel clip < ~/.ssh/id_rsa.pub
```

and go to your [GitHub settings](https://github.com/settings/ssh/new) to add
the new key.
