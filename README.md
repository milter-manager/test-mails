# test-mails

Webサイト: https://github.com/milter-manager/test-mails/

このプロジェクトは、メールシステムのテストをするためのメールを共有する
test-mailsプロジェクトです。共有したメールはオープンソースとして利用で
きるので、だれでも自分のメールシステムのテストに有効活用できます。

## はじめに

まず、どうしてこのプロジェクトが行儀の悪いメールを共有しようとするのか
という動機を説明します。

メール関連のシステムを開発している人であれば、テストのために様々なメー
ルが必要になりますよね。そのようなメールを個人で集めたり作成したりする
のは大変です。

そんなとき、自由に再利用できるテストメール集があると便利ではないでしょ
うか。メール集の各メールに対して一通り動作を確認して期待する動作をして
いれば、おおよそシステムが正しく動いていることを確認できるようなメール
集です。

このプロジェクトはテストに使えるメール集を収集し、共有します。

テストメールを共有できれば以下のようなメリットがあります。

* みんながテストで使えるメールのバリエーションが増え、網羅的なテストを
  しやすくなる。
* テストメール集はプロジェクトが管理するので各自で管理しなくてもよ
  い。このため、それぞれでバックアップをとったり、最新バージョンはどこ
  にあるかなどを調査する必要がない。プロジェクトの最新版をみればよい。

みんなでメールシステムのテストをしやすくなるように協力していきましょう!

実際にテストをしたことがある人なら今でもテストに有用なメールを持ってい
ることでしょう。その方たちがテストメールを集めることに協力してくれれば、
より多くのバリエーションを集めることができ、他のメールシステムを開発し
ている人たちにとっても有益な資産となります。

## test-mailsプロジェクトがやること

このプロジェクトでは、以下のようなメールを収集してだれでも自由に使える
ようにします。

  * 通常のメール
  * 行儀の悪いメール

行儀の悪いメールとは例えば、以下のようなメールです。

  * [RFC5321](http://tools.ietf.org/html/rfc5321)に準拠していない
  * MTAの限界を越えている
  * 日本の携帯キャリアの独自仕様が含まれているメール
  * ASCII以外のエンコーディングを使っているメール

ウィルスメールは収集対象としません。

http://www.eicar.org/ で配布されているテスト用のダミーウィルスを使用してください。

また、以下のサービスも有用です。

  * http://www.aleph-tec.com/eicar/
  * http://www.emailsecuritycheck.net/

収集したメールはMITライセンスで利用できるようにするので、非公開のメール
システムのテストにも利用できますし、使いやすいように変更したり一部だけ
切り出して利用することもできます。

まずはじめに、milter managerプロジェクトからテストメールを提供すること
をはじめました。メールシステムを構築しているかたはぜひ有意義に利用して
ください!

もし、この行儀の悪いメールを収集して共有しよう!という目的に賛同してくれ
るかたは行儀の悪いメールの収集にもご協力ください。協力方法は[協力方
法](CONTRIBUTING.md)を参考にしてください。

## ライセンス

収集したメールはMIT Licenseで提供します。

Copyright (c) 2013 The milter manager project

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
