## 参考記事

[npm workspace の使い方](https://qiita.com/frozenbonito/items/8230d4a3cb5ea1b32802)

### プロジェクト作成まで

```
❯ pwd
/path_to_directory/npm-workspace-trial
❯ npm init
❯ vi package.json // "private": true 追記
❯ npm init -w packages/server
❯ npm init -w packages/schemas
❯ npx create-react-app packages/front --template typescript
```

### schemas

```
❯ cd packages/schemas
❯ mkdir @types
❯ vi index.d.ts
```

### server

```
❯ pwd
/path_to_directory/npm-workspace-trial
❯ npm install -w packages/server --save fastify fastify-cors // add fastify
```