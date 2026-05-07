# apps-pages

個人開発アプリ用の静的ページ集（プライバシーポリシー、サポートドキュメントなど）を GitHub Pages で公開するリポジトリ。

## 公開ページ

- [Bonfire Focus プライバシーポリシー](https://da-takatsuki.github.io/apps-pages/bonfire-focus/privacy-policy.html)

## 構成

```
apps-pages/
├── README.md
└── <app-name>/
    └── privacy-policy.md
```

各アプリ用にサブディレクトリを切り、Jekyll 互換の Markdown を置く。
`---` 区切りの front matter (`layout: default` 等) があれば Jekyll が自動で HTML に変換する。
