---
name: diff
description: "mainブランチとの差分をチェックして、結果をHTMLで出力"
argument-hint: [ repositoryUrl ] [ branchName ]
---

# ブランチの名称

- リポジトリのURL$1から、mainブランチとブランチ$2の差分をチェックし、HTMLで結果を出力
- 左半分をmainブランチの表示、右半分をチェックするブランチのコードの差分として表示するスタイルで作成
- 作成フォルダは以下の命名規則に従い作成し、.aiDocsが存在しない場合は作成する

## 作成ディレクトリ、ファイルの命名規則

```
.aiDocs/[YYYYMMDD_HHMMSS]/$1_$2_diff.html
```

**例：**

- `.aiDocs/20260901_123456/gitSample_develop_diff.html`
