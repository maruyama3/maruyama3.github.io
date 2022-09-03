<script src="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.css">

The Library of maruyama3.github.io

Code4Lib JAPAN 2022 GitHub でつくるウェブサイト

## お知らせ

- 新着図書が入りました。（2022年9月3日）
- 図書館のホームページができました。（2022年9月3日）

## 八ヶ岳ブランチ

## 山中湖ブランチ

## ごあいあつ
![IMG_3248](https://user-images.githubusercontent.com/424224/188251800-e7febe34-d2fb-4535-a9c9-e32d2c8e7f8c.JPG)

リンク
[イベント情報](https://maruyama3.github.io/event)

## 新着図書

<div id="books">
  <input class="search" placeholder="検索" />
  <button class="sort" data-sort="title">
    タイトルで並べ替え
  </button>
  <ul class="list">
    <!-- _data フォルダの books.csv からデータを取り出す -->
    {% for book in site.data.books %}
      <li>
        <!-- books.csv の title 列のデータを表示 -->
        <p class="title"><a href="{{ book.url }}">{{ book.title }}</a></p>
      </li>
    {% endfor %}
  </ul>
</div>

<script>
var options = {
    valueNames: [ 'title' ]
};

var userList = new List('books', options);
</script>
