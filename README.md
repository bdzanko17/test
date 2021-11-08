# CI-CD Apache Atlas config with Gitlab-Runner on your host
- requirements: Docker, Maven, Helm, Gitlab-Runner, git
- Install Gitlab-Runner using yum package menager: https://docs.gitlab.com/runner/install/linux-repository.html
- Run Gitlab-Runner on your host: https://docs.gitlab.com/ee/ci/docker/using_docker_build.html
- sudo gitlab-runner register -n \
  --url https://gitlab.com/ \
  --registration-token REGISTRATION_TOKEN \
  --executor shell \
  --description "My Runner"
