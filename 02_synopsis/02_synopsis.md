!SLIDE

# <div class="red">あらすじ</div>
# Scalaの話
# JavaFXの話
# 今後の展望
# まとめ

<!--
ここまで5分くらいでいきたい
-->

!SLIDE

# <div class="red">あらすじ</div>

<br/>

* 某Java Champion

![pic](img/06.png "java_champion")

<!--
某日本在住のJava Championが、JavaFXに関するセッションで、
-->

!SLIDE

# <div class="red">あらすじ</div>

<br/>

* 某Java Champion

![pic](img/06.png "java_champion")

<br/>

「JavaFXやってるならプレゼンツールはJavaFXで作るのは当然ですよね(意訳)」

<!--
なるほどなーと思った。
最初に作るテーマとしてはまあアリなのかも
しかしながらガッツリ作るのは結構手間そう
できる限り手抜きして作りたい
-->

!SLIDE

# <div class="red">picture show</div>

<br/>

* https://github.com/softprops/picture-show
* markdown書くとブラウザ上でスライドとして表示してくれる

<!--
スライドをmarkdownで書いてpicture showを実行すると、
内部でWebアプリケーションサーバが立ち上がってブラウザでスライドが見れるようになる
-->

!SLIDE

# <div class="red">picture show</div>

<br/>

* こいつをWebViewでWrapすれば出来上がりでは
* 簡単そう！

<!--
と思ったが、割と色んな所で落とし穴に落ちた
ので、今日はそのへんの話をしていきたいと思います。
それやっただけじゃブラウザで確認すればよくね？な話なんですが、後で独自の機能拡張について言及します
因みに動作がもっさりしてるのは多分Rhinoのせい
Java8で動作確認してみたかったけどsbtがアバったので取り敢えず7で様子見してる
-->