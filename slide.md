### 第11回 学生エンジニア限定LT大会！！！
- - -
## 受付ちゃん（仮）をつくった  

---

### 自己紹介
- - -

* なまえ  : おしょー（学生ではない）
* Twitter : [@pink_bangbi](https://twitter.com/pink_bangbi)
* github  : [osyo-manga](https://github.com/osyo-manga)
* ブログ  : [Secret Garden(Instrumental)](http://secret-garden.hatenablog.com)
* Ruby    : Rails と戦ったり本体のパッチ書いたり    <!-- .element: class="fragment" -->
* Vim     : 100個以上のプラグインをつくったり    <!-- .element: class="fragment" -->
* C++     : 全くわからないけどたのしー    <!-- .element: class="fragment" -->
# [osushi](https://osushi.love/pink_bangbi)    <!-- .element: class="fragment" -->

---

## 受付ちゃん（仮）をつくった話

---

## 概要
- - -  

* 参加者の受付を円滑に行いたい    <!-- .element: class="fragment" -->
* conppas の参加者のチェックリストを出す    <!-- .element: class="fragment" -->
* ついでに懇親会費の徴収チェックもしたい    <!-- .element: class="fragment" -->

---

## やりたかったこと
- - -

* connpass から参加者の一覧を取得して表示    <!-- .element: class="fragment" -->
* 参加者のチェックリストを出す    <!-- .element: class="fragment" -->
* SPA(Single Page Application) + サーバサイドはなし    <!-- .element: class="fragment" -->

---

## アプリの流れ(UI)
- - -  

1. connpass の URL を入力する   <!-- .element: class="fragment" -->
1. 参加者一覧が表示される        <!-- .element: class="fragment" -->
1. 参加者をその参加者のクリックすると TODO（等）が表示される   <!-- .element: class="fragment" -->
1. 全ての TODO にチェックが入ると参加者一覧から消す   <!-- .element: class="fragment" -->

---

## デモ

https://osyo-manga.github.io/uketukechang/

---

## 技術的な話
- - -

* スクレイピング        <!-- .element: class="fragment" -->
  * connpass からデータを取得する
* レンダリング        <!-- .element: class="fragment" -->
  * SPA したい、フロントエンドで完結したい
* テンプレートエンジン        <!-- .element: class="fragment" -->
  * gh-pages で公開したい

---

## スクレイピング
- - -  

* 別のサイトにアクセスする場合は『クロスドメイン問題』がある
* この問題を解決するために YQL（Yahoo Query Language）というサービスを利用
* 古いサイトだと動かないコードが大量にあるので注意
  * http://sidewalkcafe.hatenablog.com/entry/2017/06/29/211719
* スクレイピング自体は jquery でがんばった

---

## レンダリング
- - -

* Vue.js
  * 個人的に React.js は嫌い
* Element（UI フレームワーク）
* 両方共過去に使った経験がある

---

## テンプレートエンジン
- - -

* Ruby 製の middleman を使用
* haml という HTML を簡単にかけるテンプレートエンジンが使える
* ちょっと古い…
  * 案の定、デプロイコマンドが使えなくなってた
* なんか新しいのを使いたかったけど、調べる時間がなかったので…

---

#### 所感
- - -

* 半年ぶりぐらいにフロントエンドを触ったけど結構忘れてつらかった
* <del>とはいえ、なんだかんだ一晩でできた</del>できてなかった
* 『いま○○○やるならこれ！』みたいな指標がほしい
* でもこれぐらいならさくっとつくれるよねー
* とにかく前日に慌ててつくるのはやめましょう
* やばたにえん…        <!-- .element: class="fragment" -->

---

## ご清聴
## ありがとうございました
