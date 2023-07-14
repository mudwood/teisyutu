# teisyutu
デベロッパーアプリケーションコース課題提出用

## 実行環境
デベロッパーアプリケーションコースにて構築した環境にて動作。<br>
・Mission planner<br>
・SITL<br>
・VS Code<br>
<br>
## 実行方法
１．SITLを起動<br>
２．Mission plannerを起動<br>
３．VS Codeを起動<br>
４．Mission plannerで ready to arm を確認し、VS Code 右上の実行ボタンにて起動。<br>
<br>
## 動作
１．機体と接続<br>
２．モードを GUIDED に変更<br>
３．ARM<br>
４．離陸し、高度10mまで上昇<br>
５．若干斜めに傾いた☆マーク状に飛行<br>
６．最初の点に戻ったら5秒停止<br>
７．RTL<br>
<br>
## 動作パラメータ（内部コードに直接記述）
l.75 posMag ... フライト時の倍率。mにて指定。<br>
l.77 TargetMargin ... 星状に飛ぶ際のポイントに到達したと判定する距離<br>
l.78 MoveTimeout ... 指定した点に到達するまで待つ時間。この時間を超えると次の点へ移動を開始。<br>
<br>
2023.07.14 m.doronoki.
