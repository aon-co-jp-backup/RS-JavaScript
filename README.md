# RS-JavaScript

JavaScript(ECMAScript仕様)自体のトークナイザ・パーサー・実行エンジンを、
既存のJavaScript実装コード(V8・SpiderMonkey・QuickJS等)を一切流用せず
一から開発するプロジェクト。

## 位置づけ

`RFrontEnd`エコシステム内の[`RS-TypeScript`](https://github.com/aon-co-jp/RS-TypeScript)
(型注釈削除トランスパイラ、TS風構文→JS)とは別の並行構想。RS-TypeScriptは
「型を取り除いてJSにする」だけであり、JS自体の構文解析・実行は行わない。
RS-JavaScriptはその逆——JS自体をどう解析・実行するかを担う。

## 現状(2026-09-13新設)

ひな形のみ。実装は未着手。

## 関連プロジェクト

- [RS-TypeScript](https://github.com/aon-co-jp/RS-TypeScript) — 型注釈削除トランスパイラ(TS風構文→JS)
- [RReact](https://github.com/aon-co-jp/RReact) — コンポーネントモデル(関数コンポーネント+hooks)
- [RS-BootStrap](https://github.com/aon-co-jp/RS-BootStrap) — CSSフレームワーク相当
- [RFrontEnd](https://github.com/aon-co-jp/RFrontEnd) — 親リポジトリ(全体構成)
- [open-raid-z](https://github.com/aon-co-jp/open-raid-z) — 開発ルールの正本
