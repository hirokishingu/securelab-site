# securelab-site

セキュアラボの公開ページ（2026-10-21 作成、2026-10-28 に GitHub Pages で公開）。App Store Connect の「プライバシーポリシー URL」「サポート URL」と、特定商取引法に基づく表記に使う。

| ページ | 役割 |
|---|---|
| `index.html` | アプリの紹介（マーケティング URL に使える） |
| `privacy.html` | プライバシーポリシー。アプリの設定の「プライバシー」と、リポジトリの `docs/PRIVACY_POLICY.md` と食い違わせない |
| `support.html` | よくある質問と問い合わせ先 |
| `tokushoho.html` | 特定商取引法に基づく表記（フル版の価格は「購入画面に表示する金額」。金額を決めたら書き足してもよい） |

運営者の名前・屋号・メールアドレスは、そろばんの道の公開ページ（soroban-site）と同じものを使っている。違う連絡先にするなら、全ページで置き換える（`grep -rn "hiro.apps.shoten" .`）。

規約は Apple 標準の EULA を使うので、ここには置かない。アプリは日本語だけなので、ページも日本語だけ。

## 公開先

2026年10月28日に GitHub Pages で公開した（リポジトリ hirokishingu/securelab-site の main を、そのまま配信）。main に push すると、数分で反映される。

| ページ | URL |
|---|---|
| トップ（マーケティング URL） | https://hirokishingu.github.io/securelab-site/ |
| サポート URL | https://hirokishingu.github.io/securelab-site/support.html |
| プライバシーポリシー URL | https://hirokishingu.github.io/securelab-site/privacy.html |
| 特定商取引法に基づく表記 | https://hirokishingu.github.io/securelab-site/tokushoho.html |

プライバシーポリシーを変えるときは、制定日の下に改定日を書き足し、アプリの設定の「プライバシー」とリポジトリの `docs/PRIVACY_POLICY.md` も合わせる。
