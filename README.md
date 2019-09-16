# repub
markdown 文書を 電子書籍 (epub3) に変換します。

## Install
```bash
cargo install --git https://github.com/crome110/repub
```

### Update
```bash
cargo install --force --git https://github.com/crome110/repub
```

### Uninstall
```bash
cargo uninstall repub
```

## Usage
```
$ repub --help
repub 0.1.0
Kaisei Yokoyama <yokoyama.kaisei.sm@alumni.tsukuba.ac.jp>
convert markdown(s) to epub

USAGE:
    repub [FLAGS] [OPTIONS] <input>

FLAGS:
        --help       Prints help information
        --config     設定ファイルを保存
        --save       一時ファイルを消去しない
    -V, --version    Prints version information

OPTIONS:
    -i, --bookid <book_id>       Book ID
    -c, --creator <creator>      作者、編集者、翻訳者など
    -l, --language <language>    言語
    -t, --title <title>          タイトルを設定
    -h <toc_level>               目次に表示するHeaderの最低レベル(1~5)
        --mode <writing_mode>    縦書き / 横書き [default: htb]  [possible values: htb, vrl, vlr]

ARGS:
    <input>    変換するマークダウンファイル OR 変換するマークダウン文書(複数可)の入ったディレクトリ OR 設定ファイル
```