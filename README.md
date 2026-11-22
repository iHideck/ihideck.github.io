# iHideck

iHideck の開発者のサイト（<https://ihideck.github.io/>）。運営者の名前と、公開しているアプリの一覧を載せる。Play Console に登録した組織の公式サイトとしても使う。

## 動かす・確かめる

ビルドは無い。手元で見るときは、リポジトリの直下で次を打ち、<http://localhost:8000/> を開く。`Ctrl+C` で止まる。

```sh
python3 -m http.server 8000
```

main に push すると、GitHub Pages が直下のファイルをそのまま公開する。

## 更新のしかた

アプリを足すときは、次の 2 つを行う。

1. アイコンを `icons/<アプリ名>.png` に置く
2. `index.html` の `<ul class="apps">` に、ほかのアプリと同じ形の `<li>` を 1 つ足す

## ファイル

| ファイル | 中身 |
|---|---|
| `index.html` | サイトの 1 枚だけのページ |
| `style.css` | 見た目 |
| `icons/` | アプリのアイコン |
| `googleab130f9a425a9929.html` | Google Search Console の所有者の確認のファイル。消すと確認が外れる |
| `.nojekyll` | GitHub Pages に Jekyll を通させず、ファイルをそのまま出させる |
