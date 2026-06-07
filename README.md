# pgats-ci-challenge01
## exercício 03
Leia sobre self-hosted runners/agents. Avalie: Quando faz sentido usar esse recurso? Outras plataformas oferecem recursos similares? Implemente um self-hosted agent para executar sua pipeline.
```
docker 

docker run -d --name github-runner `
  -e REPO_URL="https://github.com" `
  -e RUNNER_TOKEN="AB12CDEF34GHIJKLMNOPQRSTUVWXYZ567" `
  myoung34/github-actions-runner:latest

```