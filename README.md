# Drone CI Node Pipeline

Example Drone CI pipeline that detects changed files and runs npm install plus customizable npm run scripts.

## Getting started

### Installation

```bash
brew install drone-cli #  or scoop install drone
```

### Usage

- Command line runner requires a working `Docker` installation
- Drone executes your pipeline locally on your host machine using your local Docker daemon

#### Setup

- Place your `.drone.yml` in the root directory of your git repository
- Drone "Hello, world!":

```yaml
kind: pipeline
type: docker
name: default

steps:
- name: test
  image: alpine
  commands:
  - echo hello
  - echo world
```

#### Execute

- Execute your pipeline from the command line:

```bash
drone exec
```

## Background

## Credits

- [https://docs.drone.io/quickstart/cli/](https://docs.drone.io/quickstart/cli/)
- []()
