# nextjs-sqljs-webpack-demo

This is an example using Next.js, sql.js, Webpack5.  
This demo bundles wasm files using asset/resource.

```
const sqlWasm = (new URL("sql.js/dist/sql-wasm.wasm", import.meta.url)).toString();
const SQL = await initSqlJs({ locateFile: () => sqlWasm });
```

## Install

```
npm install
npm build
cd out
npm install http-server
```
