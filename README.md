# Website

This website is built using [Docusaurus 3](https://docusaurus.io/), a modern static website generator.

### Installation

```sh
$ yarn
```

### Build

```sh
$ ./generate_user_guides.sh
```

Above command reads the templates directory and extracts specific instructions for bevy / rust / rapier integrations.
It also injects code contained in the example files.

```sh
$ yarn build
```

Above command generates static content into the `build` directory and can be served using any static contents hosting service.

```sh
$ yarn start
```

Above command builds and starts a local development server and open up a browser window. Most changes are reflected live without having to restart the server.

### Deployment

```sh
$ GIT_USER=<Your GitHub username> USE_SSH=true yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
