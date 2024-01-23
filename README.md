# Prog2kakushin
プログラム1について
- このプログラムの概要
  - このプログラムはスマートフォンアプリ"ポケモンスリープ"のプレイをサポートするため，手持ちのポケモンをメインスキル・サブスキル・せいかくからフィルターをすることが出来るものです．
<br>実装内容としては，ポケモンの追加・ポケモンの削除・フィルター機能・現在手持ちのポケモンの閲覧です
- 作成経緯
  - 自分が現在プレイしているスマホゲーム"ポケモンスリープ"にはメインスキルによるフィルターはあるがサブスキルや性格によるフィルターがなく，少々不便であると考えていたため，pandasを用いてそれを実現するためのプログラム，および手持ちのポケモンをデータフレーム化するための要素の追加のプログラムを作成しました.
- 入力と出力について
  - ポケモン追加について｜ポケモンを追加する際にはそのポケモンの名前・メインスキル・サブスキル3つ・せいかくを入力してください．その後そのポケモンを追加したデータフレームが表示されます．同時にcsvファイルとしても保存されています．
  - ポケモン削除について｜ポケモンを削除する際には，まず現在手持ちのポケモンがインデックス付きのデータフレームとして表示されるため，その中から削除したいポケモンのインデックスを入力してください．その後そのポケモンを削除したデータフレームが表示され，csvファイルからもそのポケモンが削除された状態で保存されます．
  - フィルター機能について｜
- 工夫した点
  - サブスキルのフィルターの際にorを用いて三つの中に含まれていれば表示されるようにした点.

プログラム2について
- このプログラムの概要
  - このプログラムはいわゆる”100マス計算”の100マスの部分を可変式に、かつ出力される数字もランダムにすることによって無限に遊べるnマス計算となっています。なお、現状掛け算のみの実装となっています。
- 作成経緯
  - numpyによる配列の特性を生かした遊びを作りたいと考えており、行列式の式の特性に注目した計算プログラムを活かしたものを作成いたしました。
- 入力と出力について
  - プログラムを実行すると、まず縦何マス、横何マスで表を作られるかを聞かれるため、そこで自身が希望する数字を半角で打ち込んでください。その後、計算のための数値の上限と下限を聞かれるため先ほどと同じく希望する数字を入力してください。そうすると計算のための表が出力されます。そして左上から計算結果を入力していってください。何度か繰り返すと出力された表が見えなくなることがあるので、一定回数回答すると再び票が表示されるようになっています。
- 工夫した点
  - 最後に答え合わせを行い、正答例を出すといったような使いやすい機能の充実を行った点。

プログラム3について
- このプログラムの概要
  - このプログラムはクイズ番組などで見かけることのある、モザイクがどんどん外れていき、モザイクがかかっている画像が何なのかを当てるクイズを作成したものです。
- 作成経緯
  - python上でモザイクをかけることができ、なおかつモザイクの度合いが変わるということでこの発想に至りました。当初GIFを使う予定でしたが実装するうえで静止画を複数枚出すスタイルに変更しました。
- 入力と出力について
  - 一番上のセルは画像をダウンロードするためのセル、その次はコマンドを動かすために必要なものをimportするためのものです。三つ目のセルは例題として必ず天津飯の問題が出るようになっています。そして四つ目のセルがランダムに画像が出力され、それを当てるものとなっています。モザイクをかけられた問題を見て、その画像が何かを入力してもらいます。なお、入力する際にはひらがなで入力してください。表記ゆれを回避するためです。正解した際には正解と出力され、不正解だった場合はよりモザイクが薄くなった画像が表示されます。
- 工夫した点
  - 問題として出される画像は表記揺れが起こりづらいものを選んでいる点。
