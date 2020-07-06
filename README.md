# BookClub
読書会

読書会のリポジトリです。

いまは fluent pythonの読書をしようとしています。

下記のようなコンテンツを管理しています。

- github page は、docs の下です。
- hugoを使ってmarkdownからhtmlを生成しています。
    - contentsの下が生成する元markdownファイルの置き場所です。
- connpass用の文書置き場は ann の下です。

## 環境の作り方

### hugo

1. hugoのインストールをする。私の場合は、Debianなので

 `# apt install hugo`

1. リポジトリをcloneしてくる この時に、--recursive を忘れていると、別の手当て方法が必要になる。
1. テーマをgit submodule する。
    - see also [Hugoのテーマ「Theer」を作成しました – qqhann](https://qqhann.dev/blog/theer-stroy/)
    - themeの一個上のディレクトリに移動します。
    - git clone 時に、--recursiveを付け忘れていたら、`git submodule update --init --recursive` しましょう。
1. hugo server -D でドラフト状態のテキストを手元のブラウザで、<http://localhost:1313/BookClub/>を見ながら編集しましょう。
    - なお、新しく記事を作るなら、hugo new ファイル名です。
