# Local Storage Polyfill

The "localStorage" polyfill for Node.js.

## Acknowledgments

This repository is a fork from [@mswjs/local-storage-polyfill](https://github.com/mswjs/local-storage-polyfill>).

All credits are due to the authors of that repository.

## Usage in test environments (polyfill)

```js
// jest.setup.js
import '@franciscokloganb/local-storage-polyfill/'
```

```js
// vitest.setup.js
import { Storage } from '@franciscokloganb/local-storage-polyfill'

globalThis.window.localStorage = new Storage()
```

## Usage in Node.js environments

```js
import { Storage } from '@franciscokloganb/local-storage-polyfill'

const storage = new Storage()
storage.setItem('name', 'John')
```
