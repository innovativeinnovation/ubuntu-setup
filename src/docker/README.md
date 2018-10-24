# Docker

[Docker](https://www.docker.com/) is an open platform for developers and
sysadmins to build, ship, and run distributed applications, whether on
laptops, data center VMs, or the cloud.

### Installation

###### Via package manager

```bash
sudo apt install docker.io docker-compose
```

###### Manually

Go to https://download.docker.com/linux/ubuntu/dists/bionic/pool/stable/ and
choose `amd64`, `armhf`, `ppc64el`, or `s390x`. Download the `.deb` file
for the Docker version you want to install.

```bash
sudo dpkg -i /path/to/package.deb
```

### Configuration

If you would like to use Docker as a non-root user, you should now consider
adding your user to the "docker" group with something like:

```bash
sudo usermod -aG docker your-user
```

Remember to log out and back in for this to take effect!

### Usage

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
