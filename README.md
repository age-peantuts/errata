# 揚げピーナッツ　ホームページ

これはボードゲームサークル　揚げピーナッツのホームページ管理用のリポジトリです

## ホームページはどこでみれますか？

https://age-peanuts.github.io/age-peanuts-hp/

## 環境構築方法

- node.js > version 14.16.0
- npm > version 6.14.11

### 初回時

```bash
$ git clone git@github.com:age-peanuts/age-peanuts-hp.git
$ cd age-peanuts-hp
$ npm install
```

### 開発方法

```bash
# hot reload at localhost:3000
# 開発する際に使います
$ npm run dev
```

コード等を修正すると、自動的に再生成されてリロードされます。

## ビルド方法

```bash
$ npm run build
$ npm run generate
```
