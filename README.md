# compettition

最初に自分の好きな階層でターミナル上(windowsでこれが何に該当するかは知りません)に`git clone https://github.com/ponyopon/web_page.git` を行ってください\
VScodeならば統合ターミナルというのが開けると思うのでそれのほうが楽だと思います\
もしくは右上の緑のcodeという部分からそのままzipをダウンロードして好きな階層で解凍してください\
下にbranchの説明がありますが無理にbranch作らなくてもいい気がしています。自分のフォルダでコーディングすれば問題ないと思います。

## 開発手順
1. `git checkout main` ブランチをmainに切り替える
2. `git fetch`
3. `git pull`
4. `git checkout -b [作業内容がわかるブランチ名]`
   1. ブランチ名の先頭にはプレフィックスをつける
      1. ex) `fix/error`
5. コーディングする
   1. コミットはこまめに行う
   2. コミットする前には`git add [ファイル名]`
6.  `git push origin [作業内容がわかるブランチ名]`
7.  全ての作業を終えてpushしたら、mergeする


### コミットコメントの書き方
- レビューしやすいよう、理由と変更点を必ず記載する
  ```
  $ git commit -m "[prefix] [理由][変更点]"

  # 例
  $ git commit -m "fix: バグの修正"
  ```

- prefixはこちらを参考にする
  ```
  feat: 新しい機能
  fix: バグの修正
  docs: ドキュメントのみの変更
  style: 空白、フォーマット、セミコロン追加など
  refactor: 仕様に影響がないコード改善(リファクタ)
  ```
