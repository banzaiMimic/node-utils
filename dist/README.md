## quickstart
### js
tsconfig
```
{
  "compilerOptions": {
    "target": "es5", 
    "module": "commonjs", 
    "esModuleInterop": true, 
    "forceConsistentCasingInFileNames": true,  
    "strict": true, 
    "skipLibCheck": true,
    "outDir": "lib",
    "rootDir": "src"
  },
  "include": [
    "src/**/*"
  ]
}
```
```
const something = require('@banzaimimic/node-utils')
console.log(something.someMethod())
```

### ts
tsconfig
```
{
  "compilerOptions": {
    "module": "ES6",
    "target": "ES5",
    "lib": ["ES2020", "DOM"],
    "outDir": "./lib/",
    "moduleResolution": "node"
  },
  "include": ["src/**/*"]
}
```