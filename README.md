# vue-formatter-setting

## モチベーション

Vueのプロジェクトでフォーマッターを動作させたい。

## 実行の流れ

コード -> ESLint -> prettier の流れで動作する

コード -> prettier -> ESLint で実行する方法もあるが、これだとESLint単体で実行できないため主流ではない

## 使い方

拡張機能のインストール

```
code --install-extension dbaeumer.vscode-eslint
code --install-extension octref.vetur
```

settings.jsonをgit管理にしているので保存したタイミングで実行される。

また、コマンドからでもじっこうすることができる。

```
# lintのみでフォーマットの修正は行わない
yarn lint
# formatとlintを行う
yarn lint:fix
```

## 確認ファイル

- setting.json  
vscodeで保存時にESLintとprettierを実行する設定を書いている

- eslintrc.js  
prettierのプラグインとかを設定する

- prettierrc.js  
prettierの設定を書く

## 参考URL
- [VS CodeにPrettier・ESLint・Stylelintを導入してファイル保存時にコードを自動整形させる方法](https://wemo.tech/3307)
- [Prettier 入門 ～ESLintとの違いを理解して併用する～](https://qiita.com/soarflat/items/06377f3b96964964a65d)
- [vscode-eslint v2](https://qiita.com/mysticatea/items/3f306470e8262e50bb70)
- [Vue.jsスタイルガイドとeslint-plugin-vue検証ルールのマッピング](https://qiita.com/ota-meshi/items/85bf17494c8ea0be05d7)
- [ESLint 最初の一歩](https://qiita.com/mysticatea/items/f523dab04a25f617c87d)
- [拡張がドットファイルやドットディレクトリ以下のファイルで動作しない](https://nju33.com/vscode/eslint%20%E6%8B%A1%E5%BC%B5%E3%81%8C%E3%83%89%E3%83%83%E3%83%88%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%84%E3%83%89%E3%83%83%E3%83%88%E3%83%87%E3%82%A3%E3%83%AC%E3%82%AF%E3%83%88%E3%83%AA%E4%BB%A5%E4%B8%8B%E3%81%AE%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%A7%E5%8B%95%E4%BD%9C%E3%81%97%E3%81%AA%E3%81%84)
- [Step by Stepで始めるESLint](https://qiita.com/howdy39/items/6e2c75861bc5a14b2acf)
