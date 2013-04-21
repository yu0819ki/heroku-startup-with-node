heroku-startup-with-node
========================

HerokuでNodeするアレ

## 使い方
cloneしてHerokuに突っ込んで下さい。以下、その手順です。

## 手順
1. `$ heroku login`

  Herokuにログイン

2. `$ heroku create node-sample-627eee55c85353792b`

  Heroku上にアプリケーションを作成。30文字以内で人と被らないようにするのがつらい・・・

  わかりやすい名前の後ろに、日付をmd5した文字列をくっつけて30文字で切ってみました

3. `$ git clone git://github.com/yu0819ki/heroku-startup-with-node.git`

  必要なファイルをまとめておきました！どうぞ持って行って下さいましー

4. `$ cd heroku-startup-with-node`

  cloneしたディレクトリに移動

5. `$ git remote add heroku git@heroku.com:node-sample-627eee55c85353792b.git`

  リモートリポジトリとしてherokuを登録・・・ここちょっとよくわかってない

6. `$ git push heroku master`

  いつものデプロイ！welcome to express！


これで、あなたのHerokuでNodeする準備ができました！存分にかわいがってあげて下さいXD


### 【参考URL】
[簡単！３分でGithub上のレポジトリをherokuにpushする方法](http://dqn.sakusakutto.jp/2012/04/github-heroku-push.html)

尚、参考URLでは"--stack cedar"というおまじないを使っていますが、Heroku公式ブログにてデフォルトがcedarStackになったとのことでしたので、おまじないは要らなくなったみたいです。

[Cedarスタックがデフォルトになりました](http://blog.heroku.jp/2012/06/cedar-4947.html)
