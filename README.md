# logade

Simple minimal-config, multi-level node.js logger.

Logade is a preconfigured wrapper for the Winston package.

## Install

```ssh
npm install logade --save
```

### Usage

#### Example

```
import { getLogger } from 'logade';

const log = getLogger('api');

log.info(
    `GraphQL API Server listening on http://localhost:${api.port}! DB available at ${db.url}!`
  );
```

#### Output:

```ssh
2021-10-01 16:25:34 [info][api] GraphQL API Server listening on http://localhost:3014! DB available at http://192.168.122.211:8529!
```

The `level` is color coded, using Winston's colorize.

#### Levels

```
log.info('Infos are green');
```

```
log.error('Errors are red');
```

```
log.warn('Warnings are orange');
```
