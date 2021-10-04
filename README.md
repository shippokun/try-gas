# try-gas

gas を触ってみるべ

## 必要な Chrome 拡張

<https://chrome.google.com/webstore/detail/google-apps-script-github/lfjcgcmkmjjlieihflfhjopckgpelofo>

## 開発環境構築

```shell
npm ci
npm run login
```

## 新規開発

```shell
npm run create --title=hoge
```

新規作成時に `appsscript.json` が作成される。タイムゾーンが `America/New_York` なので、 `Asia/Tokyo` に直しておきましょう。

## 既存のプロジェクトの TS 化

1. GAS エディタの設定から スクリプト ID をコピー
2. `npm run clone id=スクリプトID`
3. close した拡張子を書き換える

## コードの更新

```shell
npm run push
```

## 注意事項

`pull` は NG です。TS→JS の変換は一方通行です。
基本的にローカルで開発し始めたら GAS のエディタは使わないこと。
