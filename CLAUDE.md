# 開発方針＆開発環境ルール(RS-JavaScript)

作業ドライブは`F:\runo`。この節は[`open-raid-z`](https://github.com/aon-co-jp/open-raid-z)の
`CLAUDE.md`を正本とし、各プロジェクトへコピーして同期する方針に準じる。

## このプロジェクトの構想(2026-09-13新設)

JavaScript(ECMAScript仕様)自体のトークナイザ・パーサー・実行エンジンを、
既存のJavaScript実装コードを一切流用せず一から開発するプロジェクト。
`RFrontEnd`傘下の`RS-TypeScript`(旧`RTypeScript`、型注釈削除トランス
パイラのみ)とは別の並行構想(ユーザー指示、2026-09-13:
「RTypeScriptとは別、JavaScript自体を新規開発」)。

## 背景

`aruaru.pro`(コンコナラ型スキルマーケットプレイス+求人サイト統合の
新規プロジェクト、Rust + RPoem + RReact軸)のフロント基盤整備の一環で
発生した、`RFrontEnd`傘下プロジェクトのネーミング統一
(`RJSON`→`RS-JSON`、`RTypeScript`→`RS-TypeScript`、`RBootstrap`→
`RS-BootStrap`、`RS-JavaScript`新設)に合わせて着手。

## 次にすべきこと

1. スコープ決定: ES仕様のどこまでを対象にするか(第一段は式評価・変数・
   関数呼び出しのみ、というのがRGraphQL/RS-JSON等の前例に沿った現実的な
   出発点)
2. トークナイザ→パーサー→AST→(まずはツリーウォーク型の)評価器、という
   最小構成から着手

## 関連プロジェクト

- [RS-TypeScript](https://github.com/aon-co-jp/RS-TypeScript) — 型注釈削除トランスパイラ(TS風構文→JS)。本プロジェクトとは役割分担
- [RReact](https://github.com/aon-co-jp/RReact) — コンポーネントモデル(関数コンポーネント+hooks)
- [RFrontEnd](https://github.com/aon-co-jp/RFrontEnd) — 親リポジトリ
- [open-raid-z](https://github.com/aon-co-jp/open-raid-z) — 開発ルールの正本
