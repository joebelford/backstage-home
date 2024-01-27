# [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn dev
```

## Upgrading

```bash
yarn backstage-cli versions:bump
```

## Add integrations

```bash
yarn add --cwd packages/backend @backstage/plugin-catalog-backend-module-github
yarn add --cwd packages/app @circleci/backstage-plugin
yarn add --cwd packages/app @backstage/plugin-kubernetes
yarn add --cwd packages/backend @backstage/plugin-kubernetes-backend
```

## Building image

```bash
yarn install
yarn tsc
yarn build:backend
yarn build-image
docker image tag backstage:latest joebelford/backstage:latest
docker push
```
