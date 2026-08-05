# 以下のルールに従ってこのアプリのプライバシーポリシーを作成する。
## ルール
- 作成したプライバシーポリシーは"PRIVACYPOLICY.html"という名前で.gitのあるプロジェクトディレクトリのルートディレクトリに必ず書き出す。
- 出力する"PRIVACYPOLICY.html"の形式は下記の `出力するHTMLファイルの中身の形式`　のセクションを必ず見てください。
- このアプリに特化したプライバシーポリシーを作成する。
- GooglePlayとAppStoreに公開するアプリなのでAppleのポリシー、Gooleのポリシー両方を最新の情報を検索しながら、必ず考慮する。
- 事業者名はkasouzouです。
- 連絡先メールアドレスは　kasouzou@gmail.comです

- 以下のすべての項目（公表事項と同意取得事項）を必ず含める
【公表事項】
・利用目的（法21条）
・オプトアウト（法27条2項）
・共同利用（法27条5項3号）
・保有個人データに関する事項（法32条1項）
（※具体的には、個人情報取扱い事業者の氏名又は名称、保有個人データの利用目的、開示等の請求等に応じる場合の手続き、苦情の申出先、安全管理措置）
・匿名加工情報に関する事項（法43条、法45条）

【同意取得事項】
・目的外利用における同意（法18条1項）
・要配慮個人情報取得時の同意（法18条2項）
・個人データを第三者提供する場合の同意（法27条1項）
・個人データを外国にある第三者に提供する場合の同意（法28条）
・個人関連情報を個人データとして取得する場合の同意（法31条1項）

- 下記のGoogleが求める条件必ず考慮する。
また、Google Playストアでは次のように定められています（2023年３月時点）。

Google Play デベロッパー販売 / 配布契約4.8
デベロッパーは、Google Play を通じて対象製品を提供するにあたり、ユーザーのプライバシーおよび法的権利を保護することに同意します。ユーザーからデベロッパーにユーザー名、パスワード、もしくはその他のログイン情報または個人情報が提供される場合、またはデベロッパーの対象製品によってそのような情報へのアクセスまたは使用が行われる場合、デベロッパーは、情報がデベロッパーの対象製品に提供されることをユーザーに認識させ、当該ユーザーについてプライバシーに関する法的に十分な通知および保護を行うことに同意します。また、デベロッパーの対象製品による当該情報の使用については、ユーザーがデベロッパーに対して許可した限定された目的のための使用のみが認められます。デベロッパーの対象製品にユーザーから提供された個人情報または機密情報が保存される場合、この保存は保護された方法で、かつ必要な範囲内でのみ行うことにデベロッパーは同意します。ただし、ユーザーがデベロッパーとの間で別途、デベロッパーの対象製品（他の製品またはアプリケーションを含まない）に直接関係する個人情報または機密情報がデベロッパーまたはデベロッパーの対象製品に保存または使用されることを許可する契約を締結することを選択した場合、デベロッパーによる当該情報の使用には当該契約の規定が適用されます。ユーザーからデベロッパーの対象製品に Google アカウントの情報が提供された場合、デベロッパーの対象製品では、ユーザーがデベロッパーに許可したタイミングで、かつユーザーがデベロッパーに許可した限定された目的にのみ、当該情報を使用してユーザーの Google アカウントにアクセスすることが認められるものとします。

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
          <h1 class="page-title">{{PAGE_TITLE}}</h1>
          <p class="page-description">{{PAGE_INTRODUCTION_TEXT}}</p>
        </header>

        <!-- 
          重要：以下の .legal-section ブロックは、規約の条項数に合わせて動的に繰り返すこと。
          各セクション内では、h2 (条名) の下に複数の p (項) を配置する形式を基本とする。
        -->
        <div class="legal-section">
          <h2>{{SECTION_NUMBER}}. {{SECTION_TITLE}}</h2>
          <p>{{PARAGRAPH_TEXT_1}}</p>
          <p>{{PARAGRAPH_TEXT_2}}</p>
          <!-- 必要に応じて項（pタグ）を増減させる -->
        </div>

        <div class="last-updated">最終更新日: {{LAST_UPDATED_DATE（○年○月○日の形式で書き込むこと。）}}</div>
      </div>
    </div>
  </main>

  <div id="footer-container"></div>
</body>
</html>
