# [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn dev
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
