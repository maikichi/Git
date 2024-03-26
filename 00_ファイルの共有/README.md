## Git（共同開発）
 ### ① Git を使う準備
Git を使う準備として[git init ]を実行する必要がある<br>
※ターミナルに出てくる「$」は入力する必要ない<br>
※「init」は「initilize」の略で「初期化」を意味している

```rb
$ git init
```

### ② 共有するファイルを選択する
ファイルを選択するには、[ git add ファイル名 ]を使う

```rb
$ git add index.html
```

### ③ 選択したファイルを記録（コミット）
選択したファイルを記録するには、[ git commit -m "メッセージ" ]を実行<br>
コミットメッセージ･･･そのコミットがどのような内容かがわかるようなメッセージにする

```rb
$ git commit -m "Create index.html"
```

### ④ リモートリポジトリの準備
リモートリポジトリを登録する際には名前を付ける必要があり、一般的には「origin」とすることが多い<br>
[ git remote add リモートリポジトリ名 URL ]とすることで登録できる

```rb
$ git remote add origin http://pro･･･
```

### ⑤ リモートリポジトリにファイルをアップロード（プッシュ）する
[ git push origin master ]とすることで、先ほど登録したリモートリポジトリにアップロードすることができる

```rb
$ git push origin master
　　　　　　　 ↑「git remote add」の時につけたリモートリポジトリ名
```

### ⑥ リモートリポジトリのファイルをダウンロード（プル）する
[ git pull origin master ]とすることで、リモートリポジトリからファイルをダウンロードすることができる

```rb
$ git pull origin master
```