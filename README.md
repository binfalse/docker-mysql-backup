# Docker MySQL-Backup

A tool to automatically dump running MySQL databases in Docker containers.

## Installation

### Manual from GitHub

Clone the [Docker MySQL-Backup repository:](https://github.com/binfalse/docker-mysql-backup)

    git clone https://github.com/binfalse/docker-mysql-backup.git

Copy the backup script to the `cron.daily` directory on your system:

    cp docker-mysql-backup/docker-mysql-backup /etc/cron.daily/docker-mysql-backup

Copy the configuration to `/etc/default/docker-mysql-backup`:

    cp docker-mysql-backup/etc/default/docker-mysql-backup /etc/default/docker-mysql-backup

### Install from my Apt repository

If you're running a Debian-based system you may want to [use my apt-repository to install the Docker MySQL-Backup tool.] In that case you just need to run

    aptitude install bf-docker-mysql-backup

Afterwards, look into `/etc/default/docker-mysql-backup` for configuration options. This way, you'll always stay up-to-date with bug fixes and new features :)

## How does that work?

You'll find [an article with detailed information on the Docker MySQL-Backup tool in my blog.](https://binfalse.de/2017/02/06/docker-mysql-update/)


