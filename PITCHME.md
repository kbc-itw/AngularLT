## 「Angular5」でWebAppを作ろう

![logo](assets/angular.png)

---

### Angularとは……

1. Google製で
2. オープンソース(MIT)な
3. Webフロントエンドフレームワーク  

---

### フロントエンドはつらいよ

HTML5 + CSS + JavaScriptは

- スケーラビリティが低い
- DOM管理とかとても煩雑
- 環境づくりがダルい

---

### スケーラビリティ

HTML5 + CSS(or SASS, LESS)  
→IDやクラスの衝突を気にする必要がある
JavaScript  
→自由すぎて大規模プロジェクトに向かない

---

### スケーラビリティ

さらに、HTML5やES6の機能は  
**ブラウザ毎に対応状況が違う**

- ES6で追加された諸々にIEは当然対応していない
- `Service Worker`はEdgeやSafariが対応してない


---

### とても煩雑

WebApp（特にSPA）ではDOMが弄られまくる  
`画面上のDOM数 * 画面数 = 全部のDOM`

**クロスプラットフォーム**だとなおさら大変  
**パフォーマンス**も気にしないといけない

---

### 環境作りがダルい

- AltJS(TypeScript, CoffeeScript, Flow, Kotlin... )
- 依存性管理(npm, bower...)
- テスト(Jasmine, Mocha, Karma, power-assart)
- ビルドツール(Grunt, Gulp, Browserify, Webpack)
- Polyfil(Babel)
- ボイラープレート(yo, BoilarPlate)

--- 

### Angularなら……

- DOMのカプセル化、フルTS利用により**スケーラブル**
- Module, Componentでの**簡潔なDOM管理**
- ツール群を一元提供する**Angular-CLI**

---

### インストール

とっても簡単。

1. Node.jsをインストール(npmを使うので)
2. コンソールを開く
3. `npm install --g @angular/cli`

ね？　簡単でしょ？

---

### プロジェクト生成

`ng new (プロジェクト名)`

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
→情報が混在

WebでAngularを調べるときは「Angular4」や「Angular5」で検索！

---

### おわり

ご清聴ありがとうございました。
