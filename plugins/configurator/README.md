# @boytecht/threeengine-configurator

Material and object configurator plugins for [ThreeEngine](https://github.com/jayhirpara28/threeengine).

```bash
npm install @boytecht/threeengine @boytecht/threeengine-configurator
```

```js
import {ThreeViewer} from '@boytecht/threeengine'
import {MaterialConfiguratorPlugin, SwitchNodePlugin} from '@boytecht/threeengine-configurator'

const viewer = new ThreeViewer({canvas: document.getElementById('canvas')})
viewer.addPluginSync(MaterialConfiguratorPlugin)
viewer.addPluginSync(SwitchNodePlugin)
```

## License

Apache-2.0. See LICENSE and NOTICE.
