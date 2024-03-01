# Docker

[Docker](https://www.docker.com/) is an open platform for developers and
sysadmins to build, ship, and run distributed applications, whether on
laptops, data center VMs, or the cloud.

## Installation

First, you need to [set up the Docker repository][dockerapt].

[dockerapt]: https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

Then, to install the latest version, run:

```bash
sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

## Configuration

If you would like to use Docker as a non-root user, you should now consider
adding your user to the "docker" group with something like:

```bash
sudo usermod -aG docker your-user
```

Remember to log out and back in for this to take effect!

## Credential stores

The Docker Engine can keep user credentials in an external credential store.
Using an external store is more secure than storing credentials in the Docker
configuration file.

You can download the helpers from the `docker-credential-helpers`
[releases page](https://github.com/docker/docker-credential-helpers/releases).

You need to specify the credential store in `$HOME/.docker/config.json` to tell
the Docker Engine to use it. For example:

```json
{
  "credsStore": "secretservice"
}
```

## Usage

To test Docker installation:

```bash
docker run hello-world
```

To list Docker images:

```bash
docker image ls
```

To list all Docker containers:

```bash
docker container ls --all
```

To list running containers:

```bash
docker ps
```

To kill all running containers:

```bash
docker kill $(docker ps -q)
```

To delete all stopped containers:

```bash
docker rm $(docker ps -a -q)
```

To delete all images:

```bash
docker rmi $(docker images -q)
```
