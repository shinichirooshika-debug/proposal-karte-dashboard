# 提案カルテ ダッシュボード（社内相談用モック）

営業メンバーが既存・休眠顧客へ提案する際に使う「顧客カルテ」に、myfolio の配信実績と Salesforce の取引情報を重ねて表示する社内Webアプリの画面案です。

- `index.html` 1ファイルで動きます（グラフは cdnjs の Chart.js、フォントは Google Fonts を読み込み）。
- タブ：全体像 / A 顧客カルテ型 / B 営業パイプライン型 / C 業態ベンチマーク型 / 社内確認事項（確認トラッカー）
- 確認トラッカーの入力内容は、GitHub Pages 版では **各自のブラウザにのみ保存** されます。共有するときは「回答一覧（表形式）」をコピーして Issue や Slack に貼り付けてください。

## 公開前の注意（必読）

このモックには **myfolio の実データ**（ごう歯科クリニックの配信実績、歯科／一般歯科の業態集計）が含まれます。

- **Public リポジトリ、または Public の GitHub Pages には置かないでください。**
- GitHub Pages を社内限定にできるのは **GitHub Enterprise Cloud の「Private Pages」（アクセス制御付き）** のみです。Free / Team プランでは、リポジトリが Private でも Pages の URL は誰でも閲覧できます。
- Enterprise Cloud でない場合は、Private リポジトリに置いて各自がダウンロードして開く運用にしてください。

## GitHub Pages での公開手順（Enterprise Cloud の場合）

1. 社内の Organization に **Private** リポジトリを作成（例：`proposal-karte-mock`）
2. `index.html` と `README.md` をリポジトリ直下にアップロード（Add file → Upload files）
3. Settings → Pages → Build and deployment で「Deploy from a branch」、Branch を `main` / `/(root)` に設定して Save
4. 同じ画面の **Visibility を「Private」** に設定（Organization メンバーのみ閲覧可）
5. 数分後に表示される URL を社内に共有

## データの出典

- myfolio：ごう歯科クリニックの配信実績、歯科／一般歯科の業態KW集計（2026年3月1日〜8月31日）
- Salesforce 項目、B案の他顧客、予算増額の試算：モック用の仮の値
