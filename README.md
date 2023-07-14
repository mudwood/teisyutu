# teisyutu
デベロッパーアプリケーションコース課題提出用

##実行環境
デベロッパーアプリケーションコースにて構築した環境にて動作。<br>
・Mission planner
・SITL
・VS Code

##実行方法
１．SITLを起動
２．Mission plannerを起動
３．VS Codeを起動
４．Mission plannerで ready to arm を確認し、
　　VS Code 右上の実行ボタンにて起動。

##動作
１．機体と接続
２．モードを GUIDED に変更
３．ARM
４．離陸し、高度10mまで上昇
５．若干斜めに傾いた☆マーク状に飛行
６．最初の点に戻ったら5秒停止
７．RTL

##動作パラメータ（内部コードに直接記述）
l.75 posMag ... フライト時の倍率。mにて指定。
l.77 TargetMargin ... 星状に飛ぶ際のポイントに到達したと判定する距離
l.78 MoveTimeout ... 指定した点に到達するまで待つ時間。この時間を超えると次の点へ移動を開始。

