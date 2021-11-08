# CI-CD Apache Atlas config with Gitlab-Runner on your host
## Configuration of Host machine
- Requirements: Docker, Maven, Helm, Gitlab-Runner, git. Install all with yum package menager
- Install Gitlab-Runner using yum package menager: https://docs.gitlab.com/runner/install/linux-repository.html
- Run Gitlab-Runner on your host: https://docs.gitlab.com/ee/ci/docker/using_docker_build.html
## Setup CI-CD pipeline
### Phases
- mvn test
- mvn publish packages to Gitlab Package registry
- build and push Docker image to Gitlab container registry
- Deploy with Helm to Openshift namespace
