# How_To
これは、宮崎ゼミのハウツーサイトに関する説明です。

プロジェクトに参加する人は、gitでアカウントを作ってユーザー名を教えてください。
gitを使いたくない人は、Codeからソースコードをダウンロードしてその中のtemplate.htmlを編集するなどして、編集したファイルをチームに共有してください。
大体の説明は、template.htmlに書いてあります。

	gitの使い方：
  https://gitforwindows.org から install
  (Windowsの人は)git CMD を開く
	git config --global user.name "ユーザーネーム"
	git config --global user.email メールアドレス
	//上の二つはしてない人だけで良いです。
  空のフォルダーに移動する。
  git init
	git clone https://github.com/Siro3150/How_To.git
	git branch ブランチ名
	git checkout ブランチ名
	編集作業
	git add .
	git commit -m 'コメントを書く'
	git push -u origin ブランチ名
  not upstream が出た時
  git pull origin
  git push -u origin ブランチ名

  origin = https://github.com/Siro3150/How_To.git の意味なので２回めからは,
  省略してoriginと書くことができると思いますが、もしエラーが出た場合は,
  ちゃんとurlを書いてください。


	２回め以降の編集作業
	git pull https://github.com/Siro3150/How_To.git
		編集作業
	git add .
	git commit -m 'コメントを書く'
	git push -u origin ブランチ名

	テンプレートの説明：
	(新しくページを作る時)
	①ファイル名は小文字英語でメインコンテンツ名.htmlとすること。(seo.html) ファイル位置はとりあえずseo.htmlと同じ階層で。
	②<meta content="">にファイル名と同じようにメインコンテンツ名を記述する。(例：seo)
	③良い感じのを<title></title>に書く(例：SEO)

	(コンテンツを追加する時)
	④サイドバーのリストにコンテンツの名前とhrefにsection番号を新たに加える。(例：sec09)
	⑤<div id="content"></div>内に以下のプログラムを加えてコンテンを記述。<section id="">に先ほどのリストに書いたsection番号を書く。

	
もっと詳しい説明：
・全体を大きくheader、content、footerに分かれておりcontentはさらにsectionごとに区切られている。
・サイドナビゲーションのリンク先をsectionのidに指定することでページ内遷移をしている。
・<div class="inner">と<div class="innerS">の違いは、innerの方が画像を含めた記事を載せるため横幅が広い。innerSの方は文章のみの説明となるので横幅が狭め
・cssとjavascriptファイルはあまり気にしなくて良い。
・後は自由に使いたいとこをコピペしたり、無駄なとこを消したりして使ってください。
