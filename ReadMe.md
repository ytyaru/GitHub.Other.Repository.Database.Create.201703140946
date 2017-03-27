# このソフトウェアについて

他者のGitHubリポジトリDBを作成する。

ライブラリ利用時にライセンス適用処理を自動化する下地として。

# 開発環境

* Linux Mint 17.3 MATE 32bit
* [SQLite3](https://www.sqlite.org/index.html) 3.8.2

## WebService

* [はてな](http://www.hatena.ne.jp/)
* [はてなAPI](http://developer.hatena.ne.jp/)

# ベース

* [GitHub.Repositories.Database.Create.20170114123411296](https://github.com/ytyaru/GitHub.Repositories.Database.Create.20170114123411296)
* [GitHub.Repository.Licenses.Database.Create.201703140912](https://github.com/ytyaru/GitHub.Repository.Licenses.Database.Create.201703140912)

Repositoriesテーブルに`Owner`列を追加した。作者のGitHubユーザ名が入る。
    
# 準備

`./Repositories/Create.sh`の以下の部分を任意のGitHubユーザ名に変更する。

```sh
GITHUB_USER_NAME=ytyaru
```

# 実行

```dosbatch
bash ./Repositories/Create.sh
```

# 結果

* `GitHub.Repositories.(other).sqlite3`ファイルが作成される
* Check.sqlに記載されたSQL実行結果がターミナルに表示される

# ライセンス #

このソフトウェアはCC0ライセンスである。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)
