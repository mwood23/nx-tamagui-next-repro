# NxTamaguiNextRepro

To reproduce:

```sh
npm install

npx nx run next:build
```

## Error One

```sh
Tamagui Webpack Loader Error:
   Cannot find module '@my/ui'
Require stack:
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/@tamagui/static/dist/extractor/loadTamagui.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/@tamagui/static/dist/extractor/createExtractor.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/@tamagui/static/dist/index.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/tamagui-loader/dist/cjs/loader.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/tamagui-loader/dist/cjs/index.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/@tamagui/next-plugin/dist/cjs/withTamagui.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/node_modules/@tamagui/next-plugin/dist/cjs/index.js
- /Users/marcuswood/burners/nx-tamagui-next-repro/apps/next/next.config.js
```

## Error Two

```sh
info  - Creating an optimized production build .✘ [ERROR] Could not resolve "common/tamagui.config"

    tamagui.config.ts:1:19:
      1 │ import config from 'common/tamagui.config';
        ╵                    ~~~~~~~~~~~~~~~~~~~~~~~

  You can mark the path "common/tamagui.config" as external to exclude it from the bundle, which
  will remove this error.
```
