# prettier-demo

[Prettier](https://prettier.io/)

## Prettierの思想

- 統一されたコードフォーマットにしたがう
- コーディングスタイル、またそのレビューに関する議論を不要に
  - 時間と体力を節約し、コードを書くことに集中できる

>It reminds me of how Steve Jobs used to wear the same clothes every day because he has a million decisions to make and he didn't want to be bothered to make trivial ones like picking out clothes. I think Prettier is like that.

## Prettierの特徴

### コードフォーマッティング

- JavaScript, including ES2017
- JSX
- Flow
- TypeScript
- CSS, Less, and SCSS
- JSON
- GraphQL
- Markdown, including GFM

### ESLintとの統合

[``eslint-plugin-prettier``](https://github.com/prettier/eslint-plugin-prettier)をつかうことで、ESLintルールに則った自動整形が可能。


**.eslintrc.json**
```.json
{
  "plugins": ["prettier"],
  "rules": {
    "prettier/prettier": "error"
  }
}
```

### エディタとの統合

Prettierには様々なエディタ用のプラグインがあり、
これらを組み込むことで指定のショートカットキーやファイル保存時の自動整形が可能になる。

それらのエディタプラグインによる整形は、Prettierで指定されているルールまたはESLintによって定められたルールに則って整形を行う。

#### Vim

https://prettier.io/docs/en/vim.html

#### Atom

```
apm install atom-prettier
```

#### VS Code

https://github.com/prettier/prettier-vscode

```
ext install prettier-vscode
```

#### WebStorm

https://prettier.io/docs/en/webstorm.html

