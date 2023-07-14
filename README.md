# IdleNecromancer [![CI](https://github.com/DeltaZen/IdleNecromancer/actions/workflows/ci.yml/badge.svg)](https://github.com/DeltaZen/IdleNecromancer/actions/workflows/ci.yml) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

An idle necromancer-themed game for WebXDC.

## Development

### Installing Dependencies

After cloning this repo, install dependecies:

```
npm i
```

### Running tests

```
npm run format:check
npm test
```

### Testing the app in the browser

To test your work in your browser (with hot reloading!) while developing:

```
npm run dev-mini
# Alternatively to test in a more advanced WebXDC emulator:
npm run dev
```

### Building

To package the WebXDC file:

```
npm run build
```

To package the WebXDC with developer tools inside to debug in Delta Chat, set the `NODE_ENV`
environment variable to "debug":

```
NODE_ENV=debug npm run build
```

The resulting optimized `.xdc` file is saved in `dist-xdc/` folder.

### Releasing

To automatically build and create a new GitHub release with the `.xdc` file:

```
git tag -a v1.0.1
git push origin v1.0.1
```
