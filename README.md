# Project report

## Project description

### Project's reporter: Uladzislau Krejzo

### Group number: md-sa2-25-23

### Pipeline. High Level Design

![project_draw](project_image.png)

### Description of application for deployment:

- Application: Jellyfin Media Server

- Programming language: C#, .NET, python

- DB: sqlite3 

## Pipeline

### Technologies which were used in project:

- Orchestration: 
Kubernetes

- Automation tools:
GitHub's action, Argo CD 

- SCM:
GitHub

- Notification:
Slack + email

- Other tools:
Helm, Docker-compose

### CI/CD description:
Developer pushing commits to the master branch with changes of app. Git Action builds docker-compose.yaml to docker image and push it to GitHub container Registry. After that Action creates a HELM diagram package and commit them to repository. Argo CD deploys application in k8s Cluster.

### Rollback flow description and implementation:

Version selection in Argo CD
Release strategy: RollingUpdate

### Perfomance of steps




### Links:

Project repository: https://github.com/jankalep/it-academy-project.git

Application site: https://jellyfin.org/

Original dockerimage: https://hub.docker.com/r/jellyfin/jellyfin 

Original jellyfin docker-compose file: https://jellyfin.org/docs/general/installation/container/

Helm repo used like example: https://github.com/brianmcarey/jellyfin-helm.git 

