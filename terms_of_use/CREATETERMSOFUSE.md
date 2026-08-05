# 利用規約を作成することが目的です。
## ルール
- 以下の①~⑬までの内容をすべて含むこと。
①利用規約全体への同意
②提供するサービスの具体的な内容
③用語の定義
④サービスを利用する際のルール
⑤違反者に対するサービスの利用停止
⑥利用規約の変更
⑦権利の帰属
⑧利用料金と支払い方法
⑨サービスの停止・変更・終了
⑩個人情報の取り扱い
⑪秘密保持
⑫損害賠償／免責事項
⑬紛争時の裁判管轄／準拠法（わたしの裁判管轄は横浜地方裁判所です。）

- 作成時は必ず"TERMS_REF.md"を参照すること。このファイルに細かい内容が書いてあります。

- 上記⑧に関してはこのアプリの特性を見て適切な書き方をすること
- 下記の`作成の手順`　に順番にしたがって作成すること
- 上記手順に従って作成した利用規約はアプリのルートディレクトリに"TERMSOFUSE.html"として切り出すこと。
- 出力するhtmlファイルの"TERMSOFUSE.html"の形式は下記の `出力するHTMLファイルの中身の形式`　のセクションを必ず見てください。


`作成の手順`
* TERMS_REF.mdの内容を読み込み、利用規約作成の順序立てをする。
* ## ルール　の項目を見て①~⑬の内容をすべて含んだ利用規約を作成する。

`出力するHTMLファイルの中身の形式`
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{PRODUCT_NAME}} | {{PAGE_TITLE}}</title>
  <link rel="icon" type="image/png" href="../../../../assets/Favicon.png">
  <link rel="stylesheet" href="../../../../styles/variables.css">
  <link rel="stylesheet" href="../../../../styles/global.css">
  <link rel="stylesheet" href="../legal.css">
  <script src="../../../../scripts/theme.js" defer></script>
  <script src="../../../../scripts/component-loader.js" defer></script>
</head>
<body>
  <div id="navbar-container"></div>

  <main class="container">
    <div class="legal-container">
      <a href="../../product.html" class="back-link">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg>
        製品一覧へ戻る
      </a>

      <div class="legal-card glass">
        <header class="page-header">
          <h1 class="page-title">プライバシーポリシー</h1>
          <p class="page-description">{{PAGE_INTRODUCTION_TEXT}}</p>
        </header>

        <div class="legal-section">
	※段落数とセクション数: セクション（.legal-section）およびその中のリスト項目や段落は、流し込むデータの量に合わせて動的に生成すること。
        </div>
        <div class="last-updated">最終更新日: {{LAST_UPDATED_DATE（○年○月○日の形式で書き込むこと。）}}</div>
      </div>
    </div>
  </main>

  <div id="footer-container"></div>
</body>
</html>­
