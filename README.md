# Vue.jsによるSPARQLエンドポイント検索アプリ

このアプリは、以前 jQueryで作成した[JavaScriptによるSPARQL利用サンプル(クエリ検索アプリ)](https://github.com/uedayou/simple-sparqlsearch-js)を[Vue.js](https://vuejs.org/)で作りなおしたものです。

使い方は、[JavaScriptによるSPARQL利用サンプル(クエリ検索アプリ)](https://github.com/uedayou/simple-sparqlsearch-js) と同じで、`index.html`内の

```
<script>
// 利用するSPARQLエンドポイントのURLを指定してください
var endpoint = "http://db.lodosaka.jp/sparql";
</script>
```

に、CORS対応のSPARQLエンドポイントのURLに書き換えるだけです。
後は、ローカルファイルとしてWebブラウザで開くか、Webサーバにindex.htmlを
コピーしてWebブラウザでアクセスしてください。

[JavaScriptによるSPARQL利用サンプル(クエリ検索アプリ)](https://github.com/uedayou/simple-sparqlsearch-js)にはない機能として、JSONファイルをダウンロードできるようになっています。
検索結果が表示されているときに、`SPARQLエンドポイント検索ページ`の右側のダウンロードボタンを押すと、ファイルがダウンロードできると思います。

## 使用モジュール

- [bootstrap](https://getbootstrap.com/)
- [axios](https://github.com/axios/axios)
- [vue-loading-overlay](https://github.com/ankurk91/vue-loading-overlay)
