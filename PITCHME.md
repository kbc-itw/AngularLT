# 「Angular5」とは

![logo](assets/angular.png)

---

### WebAppが当たり前の時代

- フロントエンド …… ブラウザで見る側
- バックエンド …… サーバ側

---

### Webフロントエンドのつらさ

HTML5 + CSS + JavaScriptは

- スケーラビリティ（拡張性）が低い
- 環境毎の対応状況が異なる
- DOM管理とかとても煩雑
- 環境づくりがダルい

---

### スケーラビリティ

HTML5 + CSS（or Sass, LESS）  
→IDやクラスの衝突を気にする必要がある  
JavaScript  
→自由すぎて大規模プロジェクトに向かない

---

### 対応状況の違い

HTML5やES6の機能は  
**ブラウザ毎に対応状況が違う**

- ES6で追加された諸々にIEは対応していない
- `Service Worker`はEdgeやSafariが対応してない

「アレを使おう！」→「ダメやん！」が多発

---

### とても煩雑

WebApp（特にSPA）ではDOMが弄られまくる  
`画面上のDOM数 * 画面数 = 全部のDOM`

**クロスプラットフォーム**だとなおさら大変  
**パフォーマンス**も気にしないといけない

---

### 環境作りがダルい

- 依存性管理(npm, bower...)
- AltJS(TypeScript, CoffeeScript, Flow, Kotlin... )
- テスト(Jasmine, Mocha, Karma, power-assart...)
- ビルドツール(Grunt, Gulp, Browserify, Webpack...)
- ボイラープレート(yo, BoilarPlate...)
- polyfill(Babel, Polyfill...)

---

### つらい 

以上で述べたところは開発の本質ではない  
つまり無駄な工数になる  
どうせ悩むならロジック部分で悩みたい

---

### 一つの解決策

![logo](assets/angular.png)

---

### Angularとは……

1. Google製で
2. オープンソース（MIT）な
3. Webフロントエンドフレームワーク  

---

### Angularなら……

- DOMのカプセル化、フルTS利用で**スケーラブル**
- 良い感じにダウンパイルして**環境対応**
- Module, Componentで**簡潔なDOM管理**
- ツール群を一元提供する**Angular-CLI**

---

### インストール

とっても簡単。

1. Node.jsをインストール
2. コンソールを開く
3. <span style="color:red";>`npm install --g @angular/cli`</span>
4. しばし待つ

ね？　簡単でしょ？

---

### プロジェクト生成

<p style="color:red;">`ng new (プロジェクト名)`</p>

これだけで

+ Angularに必要な依存関係の導入
+ README.mdの生成、git initと.gitignoreの生成
+ テスト環境の導入(Jasmine + Karma)
+ ボイラープレート生成(導入後、すぐ動かせる)

をやってくれる

---

### 実際に動かしてみるタイム

---

### 注意点

AngularJS 1.x → Angular 2.xで**互換性がなくなった**  
古い情報が混在している

WebでAngularを調べるときは「Angular4」や「Angular5」で検索！

---

### ついでに

Angularだけがjsのフレームワークではない  
（Vue.js、React.js、BackBone.js、etc...）  
問題に対し最適（と思われる）ものを選ぼう！

---

### おわり

ご清聴ありがとうございました。
