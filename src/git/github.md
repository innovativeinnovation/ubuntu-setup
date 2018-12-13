# GitHub

[GitHub](https://github.com/) is a web-based hosting service for version
control using Git.

### Connecting to GitHub with SSH

Check the [SSH section](../ssh/README.md) to see if you have any existing
SSH keys.

To add the SSH key to your GitHub account:

```bash
sudo apt install xclip
xclip -sel clip < ~/.ssh/id_rsa.pub
```

and go to your [GitHub settings](https://github.com/settings/ssh/new) to add
the new key.

### Browser Extensions

Some useful and fun browser extensions to personalize your GitHub browser
experience.

See [https://github.com/collections/github-browser-extensions](https://github.com/collections/github-browser-extensions).
