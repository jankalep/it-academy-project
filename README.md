# Project report

## Project description

### Project's reporter: Uladzislau Krejzo

### Group number: md-sa2-25-23

### Pipeline. High Level Design

![project_draw](project_image.png)

### Description of application for deployment:

- Application: Jellyfin Media Server

- Programming language: C#

- DB: MySQL 

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
Helm

### CI/CD description:
After pushing to the master branch, Git Action builds and pushes the image to GitHub container Registry, creates a HELM diagram package. Argo CD deploys application in k8s Cluster.

### Rollback flow description and implementation:

Version selection in Argo CD
Release strategy: Recreate

### Links:

Project repository: https://github.com/jankalep/it-academy-project.git

Application site: https://jellyfin.org/

Example helm repo: https://github.com/brianmcarey/jellyfin-helm.git 