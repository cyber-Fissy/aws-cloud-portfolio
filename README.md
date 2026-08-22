# AWS Cloud Portfolio

A personal cloud portfolio deployed on an Ubuntu AWS EC2 instance using Nginx, Git, GitHub, and systemd.

## Architecture

```text
Developer
   │
   │ git push
   ▼
GitHub Repository
   │
   │ systemd timer checks for updates
   ▼
AWS EC2
Ubuntu Linux
   │
   ▼
deploy.sh
   │
   │ git pull
   ▼
/var/www/projects/portfolio
   │
   ▼
Nginx
   │
   ▼
Web Browser
