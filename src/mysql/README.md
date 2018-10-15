# MySQL

[MySQL](https://www.mysql.com/) is an open-source database management system,
commonly installed as part of the popular LAMP (Linux, Apache, MySQL,
PHP/Python/Perl) stack. It uses a relational database and SQL (Structured
Query Language) to manage its data.

### Installation

```bash
sudo apt install mysql-server
```

This will install MySQL, but will not prompt you to set a password or make
any other configuration changes.

To check whether the MySQL server is running, type:

```bash
sudo systemctl status mysql
```

To install the MySQL database development files:

```bash
sudo apt install libmysqlclient-dev
```

### Security

Run the script:

```bash
sudo mysql_secure_installation
```

This will take you through a series of prompts where you can make some
changes to your MySQL installation's security options.

You should answer "y" (yes) to all questions.

### Usage

To log in to the MySQL server as root:

```bash
sudo mysql
```

To stop or start the server:

```bash
sudo systemctl stop mysql.service
sudo systemctl start mysql.service
```
