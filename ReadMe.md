# create-react-app as a Docker container

This is a dockerized version of [create-react-app] based on [`node:10-alpine`].

## Usage

```bash
alias create-react-app='docker run -it --rm -v $(pwd):/workdir -u "$(id -u):$(id -g)" -w /workdir aveltens/create-react-app'

create-react-app my-app
```

[create-react-app]: https://github.com/facebook/create-react-app
[`node:10-alpine`]: https://hub.docker.com/_/node/