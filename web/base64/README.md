# Base64
Base64は、`英数字`,`+`,`/` の合計64種類の文字で全てのデータを表すエンコード方式である。データ長を揃えるための記号として `=` が末尾に使用される。末尾が `=` , 文字数が４の倍数, この2つのどちらかが当てはまる場合Base64の可能性が高い。


## 変換方法
1. 変換したい文字列をバイナリに変換(1文字8ビット)
2. 6ビットずつに分割（満たない分は後ろに0を追加して6ビットにする）
3. 分割した6ビットを変換表を用いることで文字に変換
4. 変換した文字を4つずつに分割（足りない分は`=`を後ろに追加）

変換表や変換例は[Wikipedia](https://ja.wikipedia.org/wiki/Base64)を参照
