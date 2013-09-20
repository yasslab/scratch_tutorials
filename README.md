
## Escape from a cat! (Scratch game workshop)
```
Created by Kazuhiro Abe
abee at squeakland dot jp  

Translated by Yohei Yasukawa
yohei at yasulab dot jp
```    

This material is licensed under [CC BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/deed.ja).

### What is "Escape from a cat!" game workshop?
The game workshop of "Escape from a cat!" is a workshop that creates a game program by hands using [Scratch](http://scratch.mit.edu/), a visual programming language for kids. This document is written for facilitators of the workshop. This workshop targets for kids who have never made a program. And it takes 30 minutes at least, and takes about 2 hours if you would like to cover advanced topics.  

### Install and run Scratch
First, download and install the Scratch file that can run on your local machine from the following link.  

- [Scratch 1.4 Download](http://info.scratch.mit.edu/ja/%E3%82%B9%E3%82%AF%E3%83%A9%E3%83%83%E3%83%81_1.4_Download)

After installed, double click the cat icon (Scratch icon) and run Scratch. If you want to exit, click "Exit" from "File" in the menu bar.  
    

### Terminologies

![Table of terminologies](https://dl.dropboxusercontent.com/u/2819285/table_terminologies.png)


### First programming (making Sprite walk)　

1. For putting workshop participants in the same status, click "File" -> "New" in the menu bar. (Note: Don't use pronouns, such as "this" and "that", if possible. And repeat the instruction if needed.) You don't need to click "File" -> "New" if you have just run Scratch. If a dialog appeared to confirm saving the existing scripts, click "No". (If there is a participant who really want to save the scripts, treat individually.) Then, facilitators confirm that each participant's Scratch status is 1). selected "Motion" category, 2). no scripts in script area, and 3). a cat (Sprite) at the center of stage.
2. As a first script to make the sprite (cat) run, click the blue "move 10 steps" block from the block palette, a list of blocks in the left.  
Let participants see the sprite in the stage, and ask what happened to the sprite. (It moves to right a little.)  
If needed, explain that "a step" is equivalent to a dot. (In case that you use a projector, you will be able to see a dot, so you may let them show a dot.) As you click the block, the sprite moves 10 dots to right.  
Click the block many times until the sprite moves outside of the stage. (The point is for participants to see that clicking a block by hands is tedious.)  
When the sprite doen't move, drag the tail of it, and drop it at the center of stage.  
While dragging and dropping, facilitators need to carefully observe kids, and support them if they are difficult to manipulating a mouse, such as dragging and dragging. (But ideally, support by explaining, not by manipulating instead of them, and let them do by their hands.)
3. You can make the sprite move in this way, but it's tired, so let's make it repeat moving so that it moves without clicking the block. Now, you need to make a program. Program is a list of blocks (scripts) in order. (In this document, a program has same meaning of a script).  
To make a program, drag a "move 10 steps" block, and bring it to the script area, the gray window at the center. But just bringing the block doesn't change anything; still, it's the same situation that clicking a block makes the sprite move.  
So then, click "Control" (the top-right orange block in the top-left window), bring "forever" block to the script area, and pinch the "move 10 steps" block (you will see that the C-shaped block changes when it's close to the other block).  
If you click the "forever" block, then the sprite moves forever until it touches the edge of right side. You can drag its tails and bring it back to the center of stage, but it repeats again.  
動きを止めるには画面右上の赤い八角形のボタン(赤信号)をクリックする。ネコが止まったらドラッグして、ステージの中央に戻す。これで最初のプログラムができた(さきほどの手動操作と対比させる)。  
ファシリテーターはそれぞれのステップで子供たちの足並みが揃っているかを常に確認し、遅れていたら適宜サポート。
4. 赤信号が止まれなら、その隣の緑の旗のボタンをクリックすると動きそうだけど、動かない。  
これを動かすには、「緑の旗がクリックされたとき」ブロックを「ずっと」の上に付ける。ブロックをドラッグして近づけると、白いハイライトが表示されるので、そこで離すと合体する。  
これで緑の旗をクリックすると動き、赤信号をクリックすると止まるようになる。
5. 今度は、行きっぱなしのネコが自動的に戻ってくるようにしたい。そのためには、「動き」カテゴリーの「もし端についたら、跳ね返る」ブロックを「ずっと」の中、「10歩動かす」の下に入れる。  
緑の旗をクリックするとネコがステージを左右に往復する。  
(なにか変なことがないか聞く)ネコが右から左に進むとき、ひっくり返るのが変なので、画面中央の上、小さなネコのアイコンの左にある「↔」(左右に反転するだけ)ボタンをクリックする。
6. (まだ変なことがないか聞く)よく見ると、ネコの足が動いていない。これを動くようにしたい。  
まず、赤信号をクリックして動きを止める。  
画面中央、スクリプトエリアの上に「コスチューム」というタブがある。これをクリックするとスクリプトエリアが切り替わり、ネコの絵が2枚表示される。これがネコの衣装(コスチューム)。絵のアイコンをクリックすると、ステージのネコの絵が切り替わる(まちがえてダブルクリックするとペイントエディターが開くので、その場合は「キャンセル」で閉じる)。この切り替えを高速で行えば、パラパラマンガのように、足が動いて見えるのではないか。  
カテゴリーを「見た目」(左の上から2段目。紫色)に切り替え、「次のコスチュームにする」ブロックをクリックしてみる。すると、ネコの絵が切り替わる。つまり、このブロックをスクリプトの「ずっと」のなかに入れれば、動いて見えるはず。「次のコスチュームにする」を画面の真ん中(スクリプトエリア)にドラッグして、「ずっと」の中、「もし端についたら、跳ね返る」の下に付ける。  
緑の旗をクリックすると足を動かしながらネコが動き始める。
7. ネコが左右に動くだけでは面白く無いので、ステージ全体を動きまわるようにしたい。そのためにはネコの向きを変えれば良い。画面中央の上、小さなネコのアイコンの青い線がネコの向きを示しているので、この線をドラッグするとネコの向きが変わる。

### ネコから逃げろ！ゲームのつくり方　　

1. ネコを動かすことができたので、このネコから逃げるゲームを作る。ネコから逃げるものといえば(参加者に問いかける)、やっぱりネズミなのでそのキャラクター(スプライト)を新しく登場させる。  
そのためには、ステージの左下の「新しいスプライト:」の右に3つ並んでいる星の付いたボタンの真ん中、フォルダーのアイコンの「新しいスプライトをファイルから選ぶ」ボタンをクリックする。  
ダイアログが開いたら、そのまま「OK」ボタンをクリック(「Animals」が選ばれる)、続いて下にスクロールさせて「mouse1」をクリックしてから「OK」ボタンをクリックする。するとステージにネズミが現れる(「でかい」というリアクションが返るはず)
2. ネズミがちょっと大きすぎるので小さくする。ステージの左上に4つ並んだボタンがあるので、その右端の矢印が内側に向いているアイコンのボタン「スプライトを縮小する」をクリックする。すると、カーソルが内向きの矢印に変わるので、それでネズミを何度もクリックしてちょうどいい大きさになるまで小さくする。ネコの1/3くらいがちょうどよい。
3. ネズミの動きをプログラムする。まず、ネコと同じように「制御」の「緑の旗がクリックされたとき」と「ずっと」を真ん中の灰色のところ(スクリプトエリア)にドラッグしてつなぐ。これは基本の形で、ほとんどのプログラム(スクリプト)はこの形になる。  
ネズミは自分のキャラクター(自キャラ)なので、コントロールできるようにしたい。ここでは、マウスの操作でステージの中を動かせるようにしてみる。動かすのだからそのブロックは「動き」カテゴリーにあるはず。切り替えると上から7番目に「　▼へ行く」というブロックがある。この▼をクリックすると、メニューが開き、その中に「マウスのポインター」がある。マウスのポインターとはマウスの矢印、カーソルのこと。この項目を選ぶと「マウスのポインターへ行く」となる。このブロックを「ずっと」の中にドラッグしてはめる。プログラム全体の言葉をつなげて読むと、「緑の旗がクリックされたとき、ずっと、マウスのポインターへ行く」となる。これでよさそうなので、緑の旗をクリックしてみる。ネコが動き、ネズミをマウスでコントロールできる。
4. しかし、ネズミがネコに捕まってもなにも起こらない。そこはまだプログラムしていないから。次にそれをプログラムする。その前に、ネズミがネコに捕まるとはどういうことか考える(問いかけ)。赤信号で止めてから、ステージ上のネコとネズミが離れた位置にドラッグしてみる。これは捕まっていない。次に、ネコとネズミが重なった(触れた)状態にしてみる。これは捕まっている。つまり、ネコとネズミが触れているかどうかを調べることができれば、捕まったかどうか分かる。それには「調べる」カテゴリーのブロックを使う。
5. ブロックは沢山あるけれども、ここではネズミから見た時のネコの色(オレンジ色)に注目し、上から2番目の「■色に触れた」を使う。■をクリックすると、マウスの矢印がスポイトの形に変わるので、ネコのオレンジ色の上でクリックする。すると、その色が吸い取られて■の色が変わる。  
このブロックをスクリプトの中で使いたいけれども、このブロックは両端が尖った六角形なので、はめられる場所がない。それなので、とりあえず真ん中の灰色の空いているところにドラッグしておく。
6. 次に、ネコがネズミに捕まったとき(触れたとき)にどうなるか考える(問いかけ)。そのときは、ゲームが終了、つまり、ゲームオーバーになる。ゲームオーバーはゲームが止まって、操作しても動かなくなる状態のこと。赤信号のボタンを押した時と同じ。これを代わりに押してくれるブロックを使えば良い。「制御」の一番下にある「すべてを止める」がそれ。これもまだはめられる場所がないので、とりあえず真ん中の灰色の空いているところにドラッグしておく。
7. これで必要なブロックが揃ったので、これらをつなぎたい。そのためのブロックはないだろうか。そこで、左に並んでいる制御のブロックをみてみると、六角形の穴が開いたブロックがいくつかある。その中でも、「もし　なら」というブロックが使えそうだ。これも真ん中の灰色の空いているところにドラッグする。
8. 「もし　なら　でなければ」の六角形の穴に「■(オレンジ)色に触れた」をドラッグしてはめる。すると、「もし■(オレンジ)色に触れたなら」になる。続いて、「すべてを止める」を「もし■(オレンジ)色に触れたなら」の開いた口にはめる。すると、「もし■(オレンジ)色に触れたなら、すべてを止める」となる。
9. ここまでできたら、スクリプト全体を合体させる。「もし■(オレンジ)色に触れたならすべてを止める」の「も」をドラッグして、「ずっと」の中の一番下にはめる。スクリプト全体を読むと、「緑の旗がクリックされたとき、ずっと、マウスのポインターへ行く。もし■(オレンジ)色に触れたなら、すべてを止める」となる。これでスクリプトは完成した。
10. さっそく、緑の旗をクリックして遊んでみよう。ネコに捕まらないようにマウスを操作してネズミを動かす。ネコに捕まると全体が止まる(ゲームオーバー)。再開するには再度緑の旗を押す。(遊ぶ時間は数分程度。状況を見て判断)
11. これが簡単すぎるようなら、ネコを増やすと良い。ネコは複製(影分身)できる。ネズミの大きさを変えるときに使ったステージ左上のボタンの左端にスタンプのボタンがある。これを押してから、ネコの上でクリックすると、ネコが増える。ネコの数は全部で2匹から3匹がおすすめ。それ以上だと、難しくなりすぎる。(同じく遊ぶ時間は状況を見て判断)
12. また、それぞれのネコの速さを変えても良い。変えたいネコをステージの下の小さいアイコンから選んでから、スクリプトの「10歩動かす」の数字をクリックして、キーボードから数字を入力し、最後にEnterキーを押すと、そのネコの速さが変わる。同様にスクリプトの上のネコのアイコンの青い線をドラッグすると向きが変わる。複数のネコの動きを別々にすると難しくなる。(同じく遊ぶ時間は状況を見て判断)
13. ステージが真っ白でさびしいので、背景をつけてみる。ステージ下の小さなアイコンの左端の「ステージ」クリックし、真ん中の灰色のところの上の方にある「スクリプト」の右の「背景」タブをクリックする。「新しい背景」の右にあるボタンの中にある「読み込み」を押す。開いたダイアログでそのまま「OK」ボタンをクリック(デフォルトの「Indoors」が選択される。最初はこの中で選んでもらう)。続いて、好きな背景の絵をクリックして選んでから「OK」ボタンをクリックすると、その背景がステージにセットされる。
14. このゲームで遊ぶには、ステージを全画面にするとよい。それにはステージの右上にあるスクリーンのボタンをクリックする(発表モード)。この状態で緑の旗をクリックするとゲームがスタートする。発表モードを抜けるには、左上の曲がった矢印のボタンをクリックする。(遊ぶ時間は状況を見て判断)
15. せっかく作ったゲームもスクラッチを終了したり、パソコンのスイッチを切ると消えてしまう。そうならないように保存する。「ファイル」メニューから「名前をつけて保存...」を選ぶとダイアログが表示される。左の「デスクトップ」ボタンをクリックしてから、「新しいファイル名」の欄に作品名を入力する(デスクトップにするのは書き込み権限があるのと、作品回収を楽にするため)。作品名は、本来はその作品に合った名前を付けるべきだが、ワークショップでは、日付、ニックネーム、下の名前など、統一したルールを決めておくとスムーズ。その際、個人情報に留意すること。  
キーボード入力は、なるべく自力でやらせるようにするが、どうしても難しい子は手伝う。作品名は紙に記録させ、持ち帰って自宅や学校などで続けられるようにする。  
その他の蘭は空欄で良い。入力が終わったら「OK」ボタンをクリック。保存に成功すると、ステージの左上に作品名が表示される。  
保存した作品は「ファイル」メニューの「開く」でダイアログを開き、「デスクトップ」ボタンを押して、作品を選択して「OK」ボタンを押す。
16. この後、時間が余れば、キャラクターの絵を描きかえたり(コスチュームタブのペイントボタン。色に注意)、効果音を入れたり(音タブの録音や読み込みボタン)、スコアやタイマーを追加したりする(「変数」カテゴリー)。何をやるかは状況(子供たちの関心やノリ)で判断する。
17. スコアを作るには、ステージ下の小さなアイコンの左端の「ステージ」クリックしてから、「変数」カテゴリーの「新しい変数を作る」ボタンで「スコア」を追加する。変数関連のブロックが自動的に増え、ステージに「スコア」が表示される。
18. 「制御」に切り替えて「緑を旗をクリックしたとき」「ずっと」をつないだ基本のスクリプトを作り、「変数」に戻って、「スコアを0にする」を「緑を旗をクリックしたとき」と「ずっと」の間に入れる。同様に「スコアを1ずつ変える」を「ずっと」の中に入れる。

### 作品の共有

1. 完成した作品をインターネットで共有し、ブラウザーから遊べるようにする。事前に参加者全員で共有するアカウントを作成しておき、ログイン名とパスワードをホワイトボードやプロジェクターで掲示する(自宅で続けることを考えるとプリントで配布することが望ましい)。  
「共有」メニューの「ネットワーク上でこのプロジェクトを共有…」を選ぶと、ダイアログが表示されるので、示したログイン名とパスワード通り入力する。その他の注意事項は保存と同じ。
2. アップロード成功のダイアログが表示されたら、「OK」ボタンを「押さず」に青字の「scratch.mit.edu」のリンクをクリックする。  
失敗のダイアログが表示されたら、打ち間違いに気をつけて、再度1を行う。  
「OK」ボタンを押してダイアログを閉じてしまったときは、「共有メニュー」から「スクラッチのWebサイトを開く」を選ぶ。  
ブラウザーが開くので、ログインをクリックして、上記のユーザー名とパスワードを入力する。  
作品のサムネイルから自分の作品(ニックネーム)を探して、クリックで開く(2ページ目以降にある場合もある)。自分の作品だけでなく、他の子の作品でも遊ぶように促す。  
自宅や学校などでも、この方法で作品を開くことができる。
3. スクラッチで再度変更する場合は、「プロジェクトのダウンロード」の作品名のリンクをクリックし、ファイルをダウンロードする。このファイルをスクラッチから開くと中を見たり、直したりできる。変更したもの(リミックス)は再度共有できる。公開されたスクラッチ作品のライセンスははCC BY-SAなので、他の人の作品をリミックスしてもよい(むしろそうすべき。パクリや盗作ではないことをきちんと説明する。詳細は [遊ぶための約束](http://info.scratch.mit.edu/ja/License_to_play)を参照)。

    
  ![クリエイティブ・コモンズ・ライセンス](http://i.creativecommons.org/l/by-sa/3.0/88x31.png)  
この 作品 は [クリエイティブ・コモンズ 表示 - 継承 3.0 非移植 ライセンスの下に提供されています。](http://creativecommons.org/licenses/by-sa/3.0/deed.ja)  
