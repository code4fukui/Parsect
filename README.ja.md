# Parsect: JavaScript/TypeScript用パーサコンビネータ

**Parsect** は [TypeScript](http://www.typescriptlang.org/) や JavaScript 用のパーサコンビネータライブラリです。yacc/lex、ANTLR、PEG.js などのドメイン固有言語を使わずに、TypeScript/JavaScript のみで読みやすいパーサを簡単に記述できる方法を提供します。Parsect は TypeScript や JavaScript だけでなく、他の [AltJS](http://altjs.org/) からも利用可能です。

## 特徴

- ParsecライクなAPI
- 静的型付け: ParsectのAPIは、TypeScriptを使用することでParsecのように静的型付けされます。ただし、JavaScriptから動的型付けAPIとして利用することも可能です。
- *do記法*ライクな構文: ParsectはHaskellのdo記法に似た記述スタイルを持っています。この記法により、パーサがより読みやすくなります。
- 関数型プログラミングAPI: ほとんどの関数は参照透過です。つまり、パーサの状態を考慮する必要がありません。
- 簡単なデバッグ: パーサの途中にブレークポイントを設定し、パーサが入力をステップバイステップで消費していく様子を観察できます。
- 追加のパーサ: 正規表現パーサもサポートされています。RegExpパーサを他のパーサと組み合わせることができます。
- トークンパーサビルダー: `makeTokenParser` 関数をサポートしています。
- 式パーサビルダー: `buildExpressionParser` 関数をサポートしています。

## はじめに

### ブラウザおよびDeno向けのESモジュール

```
import { Parsect } from "https://code4fukui.github.io/Parsect/Parsect.js";
```

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
