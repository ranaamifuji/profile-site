# RETROSPECTIVE: 01 — 自己紹介サイト

実施日: 2026-07-18

## 公開情報

- ローカルで確認した: はい
- 公開 URL: https://ranaamifuji.github.io/profile-site/
- リポジトリ URL: https://github.com/ranaamifuji/profile-site

## 何を作ったか（3行以内）

名前・経歴・好きなこと・Facebookへの連絡先を掲載した自己紹介サイト。
HTMLと最小限のCSSで作成し、GitHub Pagesで一般公開した。
PC上の修正をGitの add → commit → push で公開サイトへ反映できるようにした。

## 効いた指示（コピーして残す）

1. `projects/01-profile-site の BRIEF.md を読んで実装して。完了条件をすべて満たすこと。やらないことに書いてあるものは作らない。`
2. `01-profile-site の変更を commit して GitHub に push して。`
3. 変更箇所・URL・公開確認までを具体的に指定すると、実装から検証まで一度に進められた。

## 失敗した指示・遠回り

1. Codespacesで開いた `index.html` が保存されておらず、GitHubには `README.md` しか存在しなかった。
   - 次はどう変えるか: まず `Ctrl + S`、次に `git status` で実ファイルと変更状態を確認する。
2. `git commit` の前に `git add index.html` を実行せず、`nothing to commit` になった。
   - 次はどう変えるか: `add（登録）→ commit（記録）→ push（送信）` の順を固定する。
3. すでに `01-profile-site` に移動済みなのに、もう一度同じ `cd` を実行してパスエラーになった。
   - 次はどう変えるか: ターミナル左端の現在地を確認し、移動済みなら `cd` を繰り返さない。

## 理解チェック

| ファイル | 何をしているか（3行以内） |
|----------|---------------------------|
| `index.html` | 自己紹介サイトの文章・構造・見た目を定義し、ブラウザが表示する本体 |
| `BRIEF.md` | 作る目的、掲載内容、完了条件、作らないものを実装前に決める仕様書 |
| `RETROSPECTIVE.md` | 作った後の成功・失敗・学びを次回に再利用する振り返り |
| `README.md` | リポジトリを開いた人に内容や使い方を伝える入口の説明書 |

## つまずきトップ3

1. ローカル・GitHub・GitHub Pagesが別々の場所で、保存だけでは公開サイトに反映されないこと。
2. Gitの `add`、`commit`、`push` の順番と、それぞれの役割。
3. GitHubリポジトリ、Codespaces、ターミナル、ブラウザの役割の違い。

## 次のプロジェクトに持ち越すこと

- 新しいものを作る前にBRIEFを書き、目的・操作・完了条件・やらないことを決める。
- 小さな文言修正は自分で行い、必要に応じてCursorにはcommit・push・公開確認だけを依頼する。
- エラー時は、現在地・`git status`・エラー全文を確認してから質問する。
- 学びとつまずきを日次ログへ残し、将来の初心者向けサービスの素材にする。
