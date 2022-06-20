# jenkins-stack-docker

![Visits Badge](https://badges.pufler.dev/visits/ssbostan/jenkins-stack-docker)
[![GitHub license](https://img.shields.io/github/license/ssbostan/jenkins-stack-docker)](https://github.com/ssbostan/jenkins-stack-docker/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/ssbostan/jenkins-stack-docker)](https://github.com/ssbostan/jenkins-stack-docker/stargazers)
![Twitter Follow](https://img.shields.io/twitter/follow/b9t_ir?style=social)
![LinkedIn Follow](https://shields.io/badge/style-ssbostan-black?logo=linkedin&label=LinkedIn&link=https://www.linkedin.com/in/ssbostan)

Stargaze ![GitHub Repo stars](https://img.shields.io/github/stars/ssbostan/jenkins-stack-docker?style=social) if you find it useful.

**Docker-compose** version of [jenkins-stack-kubernetes](https://github.com/ssbostan/jenkins-stack-kubernetes).

To view the complete documentation follow [jenkins-stack-kubernetes](https://github.com/ssbostan/jenkins-stack-kubernetes) repository.

## How to deploy the stack:

The stack is tested on Docker 2.10 and Docker-compose 1.26, should works on earlier versions.

### Get started:

```bash
./deploy
```

![demo](https://raw.githubusercontent.com/ssbostan/jenkins-stack-docker/master/demo.gif)

### About config docker registry
Please refer to [this link](https://docs.docker.com/registry/configuration/#list-of-configuration-options)

### Dokcer registry garbage collect
```
docker-compose exec registry sh -c "bin/registry garbage-collect /etc/docker/registry/config.yml"
```

### Docker registry UI
for more informations about this web UI refer to [this link](https://github.com/Joxit/docker-registry-ui)
![preview](https://raw.github.com/Joxit/docker-registry-ui/main/docker-registry-ui.gif "Preview of Docker Registry UI")