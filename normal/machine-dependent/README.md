# 機種依存文字

機種依存文字を含むメール。

## au-iso-2022-jp-extra-7bit.eml

丸付き数字の1が入ったメール。

エンコーディングは ISO-2022-JP。ISO-2022-JPには丸付き数字は存在しないが、
au(KDDI)独自の ISO-2022-JP には存在しているようだ。Ruby のISO-2022-JP-KDDIというエンコーディングを使って
作成した。

参考:

  * Ruby の ISO-2022-JP-KDDI について:
    http://doc.ruby-lang.org/ja/1.9.3/method/Encoding/c/ISO_2022_JP_KDDI.html

## docomo-shift-jis-extra-8bit.eml

丸付き数字の1が入ったメール。

エンコーディングは Shift_JIS。

SBMも同じエンコーディングを使用しているので、このメールを使えばSBMのケー
スもテストできる。

## emobile-utf-8-extra-base64.eml

丸付き数字の1が入ったメール。

エンコーディングはUTF-8でBase64エンコードされている。
