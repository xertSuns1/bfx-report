# bfx-report

## Setup

### Install

- install libraries. Once the project is cloned,
execute the following commands from the root directory of the project:

```
npm install
```

### Other Requirements

- Install `Grenache Grape`: https://github.com/bitfinexcom/grenache-grape:

```
npm i -g grenache-grape
```

### Сonfiguring configuration files
- all configs are stored in `./config` directory
- copy all the files with the name at the end `*.example`
- at the end of the name remove `*.example`
- сonfigure the resulting configuration files

### Run two Grapes

```
grape --dp 20001 --aph 30001 --bn '127.0.0.1:20002'
grape --dp 20002 --aph 40001 --bn '127.0.0.1:20001'
```

### Run the Grenache service

- for the production environment:

```
npm run startWorker
```

- or for the development environment:

```
npm run startWorkerDev
```

### Run the server

- for the production environment:

```
npm run start
```

- or for the development environment:

```
npm run startDev
```

### Run tests

```
npm test
```

> The launch of Grape is integrated into tests and the same ports are used
