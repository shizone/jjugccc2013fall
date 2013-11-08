!SLIDE

# あらすじ
# Scalaの話
# <div class="red">JavaFXの話</div>
# 今後の展望
# まとめ

<!--
ここまで25分くらいでいきたい
-->

!SLIDE

# <div class="red">機能の実装</div>

<br/>

* WebViewを貼り付ける
* DirectoryChooserを使う
* picture showのサーバーを起動する

<!--
picture-showのwebアプリケーションサーバーには、unfilteredを使っている
(unfilteredからJettyを使っている)
picture-showのサーバ起動ではServer#runメソッドを使っているが、これを使うと
コンソールでの入力待ちになる(キーが押されるまでサーバが起動し続ける)ため、
Server#startメソッドでサーバを起動する。
-->

!SLIDE

# <div class="red">JavaFXならではの機能追加</div>

<br/>

* カンペ機能

<!--
カンペ見せる
-->

!SLIDE

# <div class="red">カンペ機能</div>

<br/>

* スクリーンショットの表示
* カンペの表示

<!--
WebViewのスクリーンショットを取得して表示するのと、
カンペを表示している
-->

!SLIDE

# <div class="red">スクリーンショットの表示</div>

<br/>

* Timelineでディレイをかける

<!--
マウスのクリックもしくはキー入力をトリガーとして実行されるイベントに
WebViewのスクリーンショットを取得してImageに表示をすればいいだけだが、
画面のアニメーションでラグがあるため、スクリーンショットの取得に
ディレイをかける必要がある。
Timelineではプロパティを変更してアニメーションさせる他に、
特定の間隔でイベントを発生させることができる。
これを利用してスクリーンショットにディレイをかける。
-->

!SLIDE

# <div class="red">ノートの表示</div>

<br/>

* HTMLコメントをノートとして表示する
* executeScriptでHTML要素からコメントを引っ張りだしてくる

<!--
カンペの内容は、HTMLコメントから引っ張り出してくることにした
WebEngineからソースをまとめて文字列で取得できない
(構造化されたオブジェクトは取得できる)
面倒くさいのでJSぶん投げてコメントを引っ張り出してきた
executeScript:JavaFX側からブラウザにJSのコードをぶん投げる
-->

