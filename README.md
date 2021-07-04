# LECS-IzumoScience2021
図書館入室人数管理システム
自然科学部　物理班
<目的>
図書館の入退出を非接触で計測し、混雑状況をディスプレイに表示する

<条件>
-上限40人
-上限の設定人数を上回った時にわかりやすく表示する
-低コスト
-できるだけシンプルな構造　→ 他校が使えるように再現しやすくする。
-出入り口は一箇所を想定する。


<方法>

　Ⅰ.検出方法
 
　　　天井に設置したカメラで人を検知し、入室または退室したかどうかを判定する。
　-メリット
　　・利用者の負担が少ない
　　　→機械側で観測と処理を一括で行うため、生徒の日常生活に適応しやすい。
　　・集団への対応
　　　→天井から撮影するため生徒同士が重なって映らない。
　-デメリット
　　・動画撮影によるプライバシー問題
　　　→動画として保存し、インターネットに接続しないことで配慮。

　Ⅱ.処理方法
　　・Raspberry Pi と画像処理ライブラリのOpenCVを利用する。

　Ⅲ.表示方法
　　・表示用ディスプレイ:::学校の倉庫に眠っているディスプレイを活用
　　　一番目に留まりやすく、かつ簡単に表示させることができる。
　　　　-人数表示
　　　　・40人以下(グリーン)　・満員になったら(レッド)
　　　　・40人以上(イエロー)　・人数オーバー(レッド&点滅)

<材料>
　・webカメラ  １台
　・RasberryPi　１台

<参考文献>
①映像に基づく入退室カウントセンサを活用した多地点混雑情報配信サービスの開発
http://www27.cs.kobe-u.ac.jp/achieve/data/pdf/1318.pdf　神戸大学　高槻 大貴ら
②OpenCV – 背景差分で物体を検出する方法について　Pystyle
https://pystyle.info/opencv-background-substraction/


------実装機能------
・
・
・
・
・

------versions------
・v1〜v3
　　　　基礎構築
・v４
　　　　入退出検知メソッド　　基本部分完成
・v5
文字色変化
画面切り替え機能実装
画面の位置調整

・v6
人検知モジュールの分離・並列稼働
コード全体の再構築
デバッグコマンド実装

・v７
  

------参考文献------

------ ------
