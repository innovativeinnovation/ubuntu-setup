# Bitbucket

[Bitbucket](https://bitbucket.org/) is a web-based version control repository
hosting service owned by Atlassian, for source code and development projects
that use either Mercurial or Git revision control systems.

### Connecting to Bitbucket with SSH

Check the [SSH section](../ssh/README.md) to see if you have any existing
SSH keys.

To add the SSH key to your Bitbucket account:

```bash
sudo apt install xclip
xclip -sel clip < ~/.ssh/id_rsa.pub
```

and go to your Bitbucket settings to add the new key.
