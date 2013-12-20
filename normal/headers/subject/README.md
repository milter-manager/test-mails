# Subject ヘッダーに着目したメール

TODO: RFC違反のメールを含んでいるので、RFCのどの部分に違反しているのか書いてあると便利そう。

## no-subject.eml

Subject ヘッダーのないメール。

## subject-in-body.eml

Subject ヘッダーはないが、本文に Subject: で始まる行が存在しているメール。

## empty.eml

Subject ヘッダーの値が空であるメール。

## ascii.eml

Subject ヘッダーの値がアルファベットのみであるメール。

## base64-iso-2022-jp.eml

Subject ヘッダーの値が ISO-2022-JP で Base64 エンコードされているメール。

「テスト」と書かれている。

## raw-iso-2022-jp.eml

Subject ヘッダーの値が ISO-2022-JP だがエンコードされていないメール。

「テスト」と書かれている。


## raw-cp932.eml

Subject ヘッダーの値が CP932 だがエンコードされていないメール。

「①②③」と書かれている。

## raw-euc-jp.eml

Subject ヘッダーの値が EUC-JP だがエンコードされていないメール。

「テスト」と書かれている。

## raw-utf-8.eml

Subject ヘッダーの値が UTF-8 だがエンコードされていないメール。

「テスト」と書かれている。

## 90-columns.eml

Subject: ヘッダーの値が 90 桁のメール。

ヘッダーの長さも込みだと一行 99 桁ある。

## fold-after-header-name.eml

Subject: の直後に改行のあるメール。

「Subject:\n test」と書いてある。

## fold-69-column.eml

Subject ヘッダーのある行が69桁で折り返されており値が2行になっているメール。

## folded-ascii.eml

Subject ヘッダーの値がアルファベットのみで2行になっているメール。

## folded-base64-iso-2022-jp.eml

Subject ヘッダーの値が2行になっており ISO-2022-JP で Base64 エンコードされているメール。

内容は「テストテスト」

## folded-raw-iso-2022-jp.eml

Subject ヘッダーの値が2行になっており ISO-2022-JP だがエンコードされていないメール。

内容は「テスト\nテスト」

## folded-raw-cp932.eml

Subject ヘッダーの値が2行になっており CP932 だがエンコードされていないメール。

内容は「①②③\n④⑤⑥」

## folded-raw-euc-jp.eml

Subject ヘッダーの値が2行になっており EUC-JP だがエンコードされていないメール。

内容は「テスト\nテスト」

## folded-raw-utf-8.eml

Subject ヘッダーの値が2行になっており UTF-8 だがエンコードされていないメール。

内容は「テスト\nテスト」

## folded-long-lines.eml

Subject ヘッダーの値が2行になっており、1行目は99桁で折り返されているメール。
2行目は91桁ある。

内容は数字の羅列。

## folded-mime-incomplete.eml

Subject ヘッダーの値が ISO-2022-JP で Base64 で MIME エンコードされているが、一つの MIME エンコードされたブロックが2行に分かれているメール。

1行目のMIMEエンコードにJISのkanji-inコード「^$B」が、2行目のMIMEエンコードにJISのkanji-outコード「^(B」が書かれている
（1行でkanji-in/kanji-outが完結していない）

## 2-subjects.eml

Subject ヘッダーが2つあるメール。

## subject-in-body2.eml

Subject ヘッダーがヘッダー部とボディ部に1つずつ存在するメール。

## only-null.eml

Subject ヘッダーの値が NULL 文字のみであるメール。

## include-null.eml

Subject ヘッダーの値が NULL 文字を含むメール。

内容は「te\0st」
