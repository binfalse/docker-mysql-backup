# Docker MySQL-Backup

A tool to automatically dump running [MySQL](https://www.mysql.com/) and [MariaDB](https://mariadb.org/) databases in Docker containers.

## Installation

### Manual from GitHub

Clone the [Docker MySQL-Backup repository:](https://github.com/binfalse/docker-mysql-backup)

    git clone https://github.com/binfalse/docker-mysql-backup.git

Copy the [backup script](etc/cron.daily/docker-mysql-backup) to the `cron.daily` (most likely `/etc/cron.daily/`) directory on your system:

    cp docker-mysql-backup/etc/cron.daily/docker-mysql-backup /etc/cron.daily/docker-mysql-backup

Copy the [configuration](etc/default/docker-mysql-backup) to `/etc/default/`:

    cp docker-mysql-backup/etc/default/docker-mysql-backup /etc/default/docker-mysql-backup

### Install from my Apt repository

If you're running a Debian-based system you may want to [use my apt-repository to install the Docker MySQL-Backup tool.](https://binfalse.de/software/apt-repo/) In that case you just need to run

    aptitude install bf-docker-mysql-backup

Afterwards, look into `/etc/default/docker-mysql-backup` for configuration options. This way, you'll always stay up-to-date with bug fixes and new features :)

## How does that work?

You'll find [an article with detailed information on the Docker MySQL-Backup tool in my blog.](https://binfalse.de/2017/02/06/docker-mysql-backup/)
I strongly recommend to read that article before deploying the tool.

## Licence

    Docker MySQL-Backup - backup of running MySQL containers
    Copyright (C) 2016-2017 Martin Scharm <https://binfalse.de/contact/>
    
    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.
    
    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.
    
    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

