# app1

`npm create vite@latest app1 -- --template react-ts` で作ったReactのテンプレートに
以下の修正を加えたもの。

- `vite.config` を修正して、rollupでreact関連を別.jsファイルにした
- 一部のファイルをgzipして `./dist` から  `./dist-gz` にコピーする `gzipjs.js` を追加した

## S3にデプロイ

```bash
npm i
npm run build
npm run gzip
cd ../deploy
```

続きは deploy/README.md を参照


## 開発

Viteなので普通に

```bash
npm i
npm run dev
```

と

```bash
npm i
npm run build
npm run preview
```

で
