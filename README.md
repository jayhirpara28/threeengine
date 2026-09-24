# ThreeEngine

3D viewer framework for the web, built on three.js.

## Packages

| Package | Description |
|---|---|
| [`@boytecht/threeengine`](https://www.npmjs.com/package/@boytecht/threeengine) | Core viewer framework |
| [`@boytecht/threeengine-configurator`](https://www.npmjs.com/package/@boytecht/threeengine-configurator) | Material and object configurator plugins |

## Install

```bash
npm install @boytecht/threeengine @boytecht/threeengine-configurator
```

```js
import {ThreeViewer} from '@boytecht/threeengine'
import {MaterialConfiguratorPlugin} from '@boytecht/threeengine-configurator'

const viewer = new ThreeViewer({canvas: document.getElementById('canvas')})
viewer.addPluginSync(MaterialConfiguratorPlugin)
await viewer.load('model.glb')
```

## Build

```bash
npm install
NODE_ENV=production npm run build          # core -> dist/, lib/
cd plugins/configurator && npm install && NODE_ENV=production npx vite build
```

## License

Apache-2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).
