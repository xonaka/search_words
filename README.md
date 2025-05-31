# search_words

## 概要 (Overview)
`search_words` は、キーワードで素早くメモやコマンド例、設定情報などを検索できるシェルスクリプトです。キャッシュ的に使うことで、よく使う情報へ即座にアクセスできます。

A simple shell script to quickly search your frequently used notes, commands, and tips by keyword. Useful as a personal cache for daily development.

## 特徴 (Features)
- キーワードでメモやコマンド例を高速検索
- デフォルトでホームディレクトリ直下の `memo.txt` を参照
- ファイルパスを指定して他のメモファイルも検索可能
- シンプルなBashスクリプトで、どの環境でも動作

## 使い方 (Usage)

1. ホームディレクトリ直下に `memo.txt` を用意します。
2. `search_words` スクリプトを実行します。

```sh
./search_words キーワード [ファイルパス]
```
- `キーワード` : 検索したいキーワード
- `ファイルパス` : （省略可）検索対象のファイル。省略時は `~/memo.txt` を使用

### memo.txt サンプル
```
キーワード: git clone
よく使うリポジトリのクローンコマンドをすぐに参照できます。
例: git clone https://github.com/ユーザー名/リポジトリ名.git

キーワード: エラー対処
過去に遭遇したエラーとその解決策を記録しておくと、再発時にすぐ検索できます。
例: Permission denied → chmod +x ファイル名
```

## インストール (Install)
```sh
git clone https://github.com/yourname/search_words.git
cd search_words
chmod +x search_words
cp search_words ~/bin/  # またはPATHの通ったディレクトリへ
```

## コントリビュート (Contributing)
バグ報告・機能提案・プルリクエスト歓迎です！
- Issueを立ててください
- フォーク＆プルリクエストも歓迎

## ライセンス (License)
MIT License

---

## English Summary
`search_words` is a simple shell script to search your notes and command snippets by keyword. Default memo file is `~/memo.txt`. Contributions are welcome! See above for usage and details. 