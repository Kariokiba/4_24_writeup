Simple Auth IIの解法
phpのソースを読み進めていくと" $db = new PDO('sqlite:database.db');"
というのがあり自分はこれはIDなどを保存しているDBだろうなと思ったので
URLの"auth.php"のところを"database.db"に置き換えたところデータベースのダウンロードに成功。
あとは"DB Browser for SQLite"というソフトを用いて中身を覗くとフラグが書いてありました。
"FLAG_iySDmApNegJvwmxN"
問題6の解法
パケットの動きを見ているとFTPの通信をしているようだったのでFTP関連のみを表示するようにフィルターを掛けて絞る
すると1.txt,2.zip,3.txtzipというのがありました。ZIPはそのままでは読めないのでいったんファイルとして保存して中身を見ました。
そこで得た文字列ファイルの連番順に結合することでフラグを得られました
"ctf4b{This_communication_is_not_encrypted.}"