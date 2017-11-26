@title[表紙]
# 「Angular」で作るWebアプリケーション

![logo](assets/angular.png)

---

@title[WebApp作りのめんどいところ]
## Webアプリケーションを作るにあたり

HTML5 + CSS + JavaScriptは

- スケーラビリティが低い |
- DOM管理とかとても煩雑 |
- 環境づくりがダルい |

---

## スケーラビリティ

<dl>
  <dt>HTML5 + CSS(or SASS, LESS)</dt>
  <dd>IDやクラスの衝突を気にする必要がある</dd>
  <dt>JavaScript</dt>
  <dd>自由すぎて大規模プロジェクトに向かない</dd>
</dl>

これに加え、HTML5やES6の機能は**ブラウザごとに対応状況が違う**

+ ES6で追加された諸々にIEは当然**対応していない**
+ `Service Worker`はEdgeやSafariが対応してない

→ Can I use it問題がつきまとう

---

## とても煩雑

Webアプリケーション（特にSPA）ではDOMががっちゃんがっちゃん弄られまくる
再利用性の低い仕様で
`画面上のDOM数 * 画面数 = 全部のDOM`
を管理できるのか問題

**クロスプラットフォーム**になるとなおさら大変
しかも**パフォーマンス**を気にしないと(JQueryなんかは遅い……）

---

## 環境作りがダルい

+ AltJS(TypeScript, CoffeeScript, Flow, Kotlin... )
+ 依存性管理(npm, bower...)
+ テスト(Jasmine, Mocha, Karma, power-assart)
+ ビルドツール(Grunt, Gulp, Browserify, Webpack)
+ Polyfil(Babel)
+ ボイラープレート(yo, BootStrap)

--- 

@title[Angularというソリューション]
## Angularなら……

![logo](assets/angular.png)

Angularは開発環境まで含めたフレームワーク

- DOMのカプセル化、TypeScript利用による**スケーラビリティ** |
- Module, Componentの概念によりすっきりと**管理**(再利用性も高い！) |
- ツール群をワンストップで用意できる**Angular-CLI**


---

@title[インストール方法]
## インストール

とっても簡単。

1. Node.jsをインストール(npmを使うので) 
2. コンソールを開く
3. `npm install --g @angular/cli`

ね？　簡単でしょ？

---

@title[プロジェクト生成]

とっても簡単。

`ng new (プロジェクト名)`

これだけで

+ Angularに必要な依存関係の導入
+ README.mdの生成、git initと.gitignoreの生成
+ テスト環境の導入(Jasmine + Karma)
+ ボイラープレート生成(導入後、すぐ動かせる)

をやってくれる

---

@title[動かしてみる]

## 実際に動かしてみるタイム

---

@title[注意]

## 注意点

AngularJS 1.x → Angular 2.xで**互換性がなくなった**
(ついでに名前も変わった)
WebでAngularを調べるときは「Angular4」や「Angular5」で検索！

--- 

## おわり

ご清聴ありがとうございました。