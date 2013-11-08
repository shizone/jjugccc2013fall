!SLIDE

# あらすじ
# <div class="red">Scalaの話</div>
# JavaFXの話
# 今後の展望
# まとめ

<!--
ここまで10分くらいでいきたい
-->

!SLIDE

# <div class="red">sbtの設定</div>

<!--
Scalaの話というかsbtとその周りの話をします
Scalaのビルドツールであるsbtの設定をする
ご存じない方のために行っておくとsimple build toolらしいです。
もはやsimpleとは程遠いですが、その分強力なツールです。
-->

!SLIDE

# <div class="red">sbtの設定</div>

<br/>

* JavaFXを使えるようにする

<!--
sbtでjavafxrt.jarにパスが通らないので通すための設定をする
-->

!SLIDE

# <div class="red">sbtの設定</div>

<br/>

* 設定ファイルでclasspathの設定
* http://stackoverflow.com/questions/14123749/how-to-detect-javafx-runtime-jar-in-sbt

<!--
・設定ファイル見せる
Stackoverflowで見つけたJAVA_HOMEから辿る方式を採用
sbtの設定ファイルは複数作っても全部読んでくれるので、この設定だけを行うファイルを作ってしまうと良い
他にもjavafxrt.jarをunmanagedなライブラリに突っ込んでしまうという手もある
OpenJDKの8眺めてたらなかったのでこの辺統合されるんスかね？
詳しい人がいたら教えてください。
-->

!SLIDE

# <div class="red">JavaFXを使えるようにする</div>

<br/>

* giter8テンプレート作った
* https://github.com/n8han/giter8
* https://github.com/shizone/scala-javafx-fxml.g8
* $ g8 shizone/scala-javafx-fxml

<!--
この辺の設定ファイルを入れてあるgiter8テンプレートを作成してあります
giter8とは、GitHub上にテンプレートのプロジェクトを作成してそれを指定すると、
対話形式プロジェクト名とかScalaのバージョンを答えるとプロジェクト作成してくれるツール
2行目がgiter8のURL
3行目が作成したテンプレート
UIの部分はScalaFXを使わずにふつうにFXMLでゴリゴリやってます
-->

!SLIDE

# <div class="red">picture showの取り込み</div>

<br/>

* Full Configuationのdependenciesを使う

<!--
プロジェクトファイル見せる
dependenciesでリポジトリのURLを指定すると、
ビルド時にソースを取得して一時ディレクトリに配置し、ビルドしてパスに加えてくれる
ワークのディレクトリ見せる
(~/.sbt/staging)
依存プロジェクトはsbtのプロジェクトである必要がある
(ネストされたsbtプロジェクトのような形になる)
マルチプロジェクトの場合、サブプロジェクトを指定する
sbtのプロジェクトがネストされた形になっている
で、これでpicture showがプロジェクトに取り込まれた形になったが、
picture showが使用しているの依存ライブラリが見つからない
(該当のバージョンがresolverのリポジトリから消えている)
ため、ビルドに失敗する！！
んで、仕方なく
-->

!SLIDE

# <div class="red">picture showの取り込み</div>

<br/>

* Fork(無念の)

<!--
Forkします
完全に敗北した気分です
で、更に
-->

!SLIDE

# <div class="red">picture showの取り込み</div>

<br/>

* picture-showのバージョンに合わせた形で2.9.2に(無念の)

<!--
Forkしたので設定ファイルのバージョン指定と依存ライブラリのバージョンを
見なおしたらもしかしたら動くかも知れないけど、まだ試してない
-->

