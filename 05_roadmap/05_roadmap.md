!SLIDE

# あらすじ
# Scalaの話
# JavaFXの話
# <div class="red">今後の展望</div>
# まとめ

<!--
ここまで40分くらいでいきたい
時間があればやる
-->

!SLIDE

# <div class="red">今後の展望</div>

<br/>

* conscriptの対応
* ハッシュタグの表示
* 関連URLとかの投下機能

!SLIDE

# <div class="red">conscriptの対応</div>

<br/>

* https://github.com/n8han/conscript
* GitHub上にあるScalaアプリを自動で取得してbuild/publishしてくれるツール
* cs shizone/tengu
* それ用の設定を追記する

!SLIDE

# <div class="red">ハッシュタグの表示</div>

<br/>

* ハッシュタグを字幕風に表示したい
* 昔そういうChrome Extension作ってた(API1.0の頃…)

!SLIDE

# <div class="red">ハッシュタグの表示</div>

<br/>

* そんな時のためのTwitter4J

!SLIDE

# <div class="red">ハッシュタグの表示</div>

<br/>

* <del>そんな時のためのTwitter4J</del>
* そんな時のためのTwitter4S

!SLIDE

# <div class="red">ハッシュタグの表示</div>

<br/>

* <del>そんな時のためのTwitter4J</del>
* そんな時のためのTwitter4S
    * Twitter4JのWrapper
    * https://github.com/Shinsuke-Abe/twitter4s
    * 中の人：あべさん
    * #ccc_r26 で握手

<!--
Twitter4SはTwitter4JのWrapper
-->

!SLIDE

# <div class="red">関連URLの投下機能</div>

<br/>

* 特定のページを表示した時に、そこに書いてるURLをTwitterとかで簡単に投下したい
* そんな時のた(ry
    * 中の人：あ(ry
    * #ccc_r26 で握手

!SLIDE

# <div class="red">関連URLの投下機能</div>

<br/>

* コメントの中に独自の構文を作って投下する文言を記述する？
* そいつを使ってPost or 投稿画面を表示

<!--
パーサーコンビネータとか使ってもいいけど、この程度であれば正直正規表現でゴリったほうが早い気がする
-->

!SLIDE

# <div class="red">が、</div>

<br/>

* やる前に飽きそうな気がする
