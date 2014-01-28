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

Subject ヘッダーの値が ASCII 以外の文字なので、 [RFC 2047][] に従ってフォーマットしているメール。

「charset」は「ISO-2022-JP」で、「encoding」は「B」を使っている。

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

Subject ヘッダーの値が2行になっているメール。ヘッダーの値が ASCII 以外の文字なので、 [RFC 2047][] に従ってフォーマットしている。

「charset」は「ISO-2022-JP」で、「encoding」は「B」を使っている。

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

Subject ヘッダーの値が ASCII 以外の文字なので、 [RFC 2047][] に従ってフォーマットしているメール。

「charset」は「ISO-2022-JP」で、「encoding」は「B」を使っている。ただし、 Base64 エンコードされたブロックが2行に分かれている。

1行目のBase64エンコードされたブロックにISO-2022-JPのdouble-byte-seq「^$B」があり、2行目のBase64エンコードされたブロックにISO-2022-JPのsingle-byte-seq「^(B」がある。

（1行でdouble-byte-segmentが完結していなくて、2行目もdouble-byte-segmentが継続している。）

参照: [RFC 1468][] （ISO-2022-JPのRFC）

## 2-subjects.eml

Subject ヘッダーが2つあるメール。

## subject-in-body2.eml

Subject ヘッダーがヘッダー部とボディ部に1つずつ存在するメール。

## only-null.eml

Subject ヘッダーの値が NULL 文字のみであるメール。

## include-null.eml

Subject ヘッダーの値が NULL 文字を含むメール。

内容は「te\0st」

  [RFC 1468]: http://tools.ietf.org/html/rfc1468
  [RFC 2047]: http://tools.ietf.org/html/rfc2047
