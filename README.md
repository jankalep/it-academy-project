## Project report

### Project's reporter: Uladzislau Krejzo

### Group number: md-sa2-25-23

## Description of application for deployment:

- Application: WordPress 6.2/2

- Programming language: PHP

- DB: MySQL 

- Link on git repository: https://github.com/jankalep/it-academy-project.git

## Pipeline

## Technologies which were used in project:

- Orchestration: 
Kubernetes

- Automation tools:
GitHub's action, Argo CD 

- SCM:
GitHub

- Notification:
Slack

- Other tools:
 Docker, Helm

## CI/CD description:
After pushing to the master branch, Git Action builds and pushes the image to GitHub container Registry, creates a HELM diagram package. Argo CD deploys application in k8s cluster.

## Rollback flow description and implementation:

Version selection in Argo CD


## Links:

Project repository: https://github.com/jankalep/it-academy-project.git


![project_draw](project_image.png)
