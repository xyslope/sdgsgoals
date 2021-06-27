# sdgsgoals
Export SDGs Goals in various formats.

We would be pleasure to merge our output to other project if we find similar projects.

# Japanese Version
## SDGsの目標をテキストやCSVに
よく探すので、使いやすいフォーマットでまとめておく。

和訳はIGESによる仮訳が外務省の[https://www.mofa.go.jp/mofaj/files/000101402.pdf](Webサイト)にある。
本プロジェクトは、この目標を使いやすいフォーマットに変換することを目的とする。

### フォーマット
データはorgで管理する。
ここから、markdown, word, excelに変換する。

### 出力する文書
- 目標のみ
- 目標と指標
- 目標と解説

などを予定。

### 作業工程
IGES仮訳のPDFをまず、テキストに変換する。
それが、GoalAndTargetsJPsource.txt。
このファイルは、変換ミスや判定しきれない改行コードなどがあるので、これをまず整形する。

そのために、まずGoalAndTargetsJP.orgを生成し、作業を行う。

- 目標をトップレベルのパラグラフとし、指標（Targets ）を第二レベルのパラグラフに変換する。
- 不要な改行を削除
- 不要な空白を削除（エクスポートには反映されないので、気にする必要はない）
- ハードコードされているページ番号を削除
- ファイルを編集した後、変換はスクリプトを作成したほうがよい
