## v-server-setup

# Description

In diesem Projekt wurde ein V-Server eingerichtet und abgesichert.
Ein SSH-Key-Pair wurde lokal erstellt und der Public Key auf dem Server hinterlegt. Der Passwort-Login wurde deaktiviert, sodass der Zugriff nur noch per SSH-Key möglich ist.

Der Webserver NGINX wurde installiert, konfiguriert und zeigt eine angepasste HTML-Startseite an.

Git wurde mit Benutzername und E-Mail eingerichtet. Zusätzlich wurde ein SSH-Key auf dem Server erstellt und in GitHub hinterlegt, um Repositories per SSH nutzen zu können.

# Table of Contents

- [Prerequisites](#prerequisites)
- [Quickstart](#Quickstart)
- [Usage](#Usage)

# Prerequisites

- Ready to use VM
- SSH public & private key
- Git SSH connection


# Quickstart

- clone the repository by using "git clone git@github.com:FlyingChris1/v-server-setup.git"

- Update and install Nginx with "sudo apt update && sudo apt install -y nginx"


# Usage

### Generate a ssh key pair

ssh-keygen -t ed22519

### SSH alias

alias (aliasName)="ssh -i ~/.ssh/localkey (UserName)@(IP)"

### Disable password Login

sudo nano /etc/ssh/ssh_config

### Create html document for Webserver

sudo touch /var/www/alternatives/alternate-index.html

### Create directory

mkdir /var/www/alternatives








