# Parsect: Parser Combinator for JavaScript/TypeScript

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

**Parsect** is a parser combinator library for [TypeScript](http://www.typescriptlang.org/) or JavaScript. It provides an easy way to write a readable parser in only TypeScript/JavaScript without any other domain-specific languages like yacc/lex, ANTLR or PEG.js. Parsect can be used not only from TypeScript and JavaScript but also other [AltJS](http://altjs.org/)s.

## Features

- Parsec-like API
- Statically typed: The API of Parsect is statically typed like Parsec with TypeScript. However, you can also use it from JavaScript as a dynamically typed API.
- *do-notation* like syntax: Parsect has Haskell's do-notation-like notation style. This notation makes a parser more readable.
- Functional Programming API: Most of the functions are referentially transparent. It means you don't need to consider the states of your parsers.
- Easy debugging: You can set a breakpoint in the middle of your parser and watch the parser consume the input step-by-step.
- Extra parsers: A regular expression parser is also supported. You can combine RegExp parsers with other parsers.
- Token parser builder: `makeTokenParser` function is supported.
- Expression parser builder: `buildExpressionParser` function is supported.

## Getting Started

### ES module for Browsers and Deno

```
import { Parsect } from "https://code4fukui.github.io/Parsect/Parsect.js";
```

## License

MIT License — see [LICENSE](LICENSE).