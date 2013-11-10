!SLIDE

# <div class="red">R2-5 ScalaでJavaFXのWebViewを愛でる試み</div>

<br/>

2013/11/09(Sat)

<br/>

#jjug\_ccc #ccc_r25

<!--
最初にScalaとJavaFXのレベル感を確認しておきたい
マサカリ歓迎
間違ってるところとかより良い解決方法があったら教えてください
皆さんの声援がこのセッションの完成度をあげます
-->

!SLIDE

# <div class="red">About me</div>

<br/>

@razon

すみだゆうき

もじゃ変

![pic](img/01.png "twitter") 

<!--
すみだと申します。
なぎせさんのパチモノ感満載ですが特に関係はありません。
もじゃもじゃした変態なのでもじゃ変とか呼ばれています。
Twitter垢をﾋｮﾛｰしても非技術的な発言とエアリプライの嵐なのであまりｵﾇﾇﾒできません。
-->

!SLIDE

# <div class="red">大都会岡山から来ました</div>

<br/>

![pic](img/02.png "njslyr") 

<!--
ニンジャ修道会の聖地、岡山県から来ました
わからない人はニンジャスレイヤーを全巻購入してください。
書籍版ではまだニンジャ修道会は出てきません。
-->

!SLIDE

# <div class="red">大都会岡山から来ました</div>

<br/>

* 天領倉敷Scala
* 岡山Javaユーザ会

<!--
今回はふたつの勉強会の所属として来たので、軽く紹介を
-->

!SLIDE

# <div class="red">天領倉敷Scala</div>

<br/>

![pic](img/03.png "tkscala")

<!-- 
天領倉敷Scalaは岡山県倉敷市を拠点とする小さなScala勉強会
3年くらいやってます
だいたいこんな開催規模です
これは極端ですが、まあ5人くらいの規模
 -->

!SLIDE

# <div class="red">天領倉敷Scala</div>

<br/>

![pic](img/04.png "kwkni_scala")

<!-- 
東京の勉強会だとこんなもんです
うらやましい。
 -->

!SLIDE

# <div class="red">岡山Javaユーザ会</div>

<br/>

* JJUG CCC 2013 Spring

<br/>

![pic](img/05.png "2013spting")

<!-- 
実は、岡山Javaユーザ会に所属している人間が春のJJUG CCCで登壇しています
地方における勉強会事情
 -->

!SLIDE

# <div class="red">岡山Javaユーザ会</div>

<br/>

* JJUG CCC 2013 Spring

<br/>

![pic](img/05.png "2013spring")

(但しPHPer)

<!-- 
が、こいつはPHPerです
別に殺さなくてもいいです
代表も転職したせいで最近Railsしか触ってないとか、
他のメンバーも東京にドナドナされたりとか緑色のアンチクショウでお馴染みの
携帯端末のJavaやってるぜとかそんなんなので、割と僕が最後の砦です。
-->

!SLIDE

# <div class="red">本日のおしながき</div>

<br/>

* あらすじ
* Scalaの話
* JavaFXの話
* 今後の展望
* まとめ

<!-- 
・今回話すことですが、
・お題を決めたきっかけ
・Scala側でのポイント
・JavaFX側でのポイント
(時間があればやる)
そして、今回話すテーマはこのプレゼンテーションツールのことなのですが、
その今後の展望をお話しようと思います。
因みに、ScalaにせよJavaFXにせよそんなに突っ込んだ(難しい)話はしません。
ちょっと触ったくらいのレベルで問題ないと思います。
-->

