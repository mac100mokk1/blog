---
layout: post
title: AozoraEPUB3に対応サイトを自力で追加してみた(2017/9/27)
---

アルファポリスの小説をEPUB化したかったがアプリが見つけられなかった...  
小説家になろうのダウンロードでよく使っているAozoraEPUB3が比較的簡単にサイトを追加できそうだったので作って見た。


使い方
--

1. このプロジェクト全体を[ダウンロード](https://github.com/mac100mokk1/add-aozoraEPUB-site/archive/master.zip)  
※ダウンロードからダウンロードできない場合はgithubからダウンロードしてください  
2. ダウンロードしたファイルを展開
3. 必要なサイトのドメイン名のフォルダをAozoraEPUB3.jarと同ディレクトリにあるwebフォルダにコピー
4. いつもと同じようにAozoraEPUB3をつかいます

リクエストや問題点の報告について
---
リクエストや問題点等の報告は[ここ](https://github.com/mac100mokk1/add-aozoraEPUB-site/issues)にしていただけると対応するかもしれません  

ToDo
---
ルビに対応させたい  
原因は明らか出るが原因の修正をextract.txtの編集で済ます方法を私は知らない。  
ソースを見て推測してみると  
`<ruby><rb>るび</rb><rp>(</rp><rt>フリガナ</rt><rp>)</rp></ruby>`  
や  
`<ruby><rb>るび</rb><rp></rp><rt>フリガナ</rt><rp></rp></ruby>`  
であれば問題なくルビに変換されるが、アルファポリスでの書式が  
`<ruby>るび<rt>フリガナ</rt></ruby>`  
であることが推測できた。  
はじめてjavaに挑む必要があるかもしれない  




変更履歴
--
2017/9/27 作成


last update:2017/9/29
