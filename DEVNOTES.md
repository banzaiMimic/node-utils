### node-externals
exclude deps from a lib that you will offload reqs to child packages [express ect. [read more](https://www.npmjs.com/package/webpack-node-externals) ]

./webpack.config.js
```
const
  ...
  nodeExternals = require('webpack-node-externals') 
  
module.exports = {
  ...
  target: 'node',
  externals: [nodeExternals()],
  ...
}
```

## yarn linking
if you need to test changes locally into an external project
```
yarn build
yarn link
```
go to root of other project
```
yarn link @banzaimimic/node-utils
```