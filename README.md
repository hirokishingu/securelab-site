# securelab-site

セキュアラボの公開ページの下書き（2026-10-21 作成。まだ公開していない）。App Store Connect の「プライバシーポリシー URL」「サポート URL」と、特定商取引法に基づく表記に使う。

| ページ | 役割 |
|---|---|
| `index.html` | アプリの紹介（マーケティング URL に使える） |
| `privacy.html` | プライバシーポリシー。アプリの設定の「プライバシー」と、リポジトリの `docs/PRIVACY_POLICY.md` と食い違わせない |
| `support.html` | よくある質問と問い合わせ先 |
| `tokushoho.html` | 特定商取引法に基づく表記（フル版の価格は「購入画面に表示する金額」。金額を決めたら書き足してもよい） |

運営者の名前・屋号・メールアドレスは、そろばんの道の公開ページ（soroban-site）と同じものを使っている。違う連絡先にするなら、全ページで置き換える（`grep -rn "hiro.apps.shoten" .`）。

規約は Apple 標準の EULA を使うので、ここには置かない。アプリは日本語だけなので、ページも日本語だけ。

## 公開のしかた（オーナーが決めてから）

```sh
gh repo create hirokishingu/securelab-site --public --source . --push
gh api -X POST repos/hirokishingu/securelab-site/pages -f 'source[branch]=main' -f 'source[path]=/'
```

数分後に https://hirokishingu.github.io/securelab-site/privacy.html が開く。制定日（各ページの「2026年10月21日 制定」）は、公開した日に直す。
