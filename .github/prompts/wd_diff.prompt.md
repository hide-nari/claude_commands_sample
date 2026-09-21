---
name: wd_diff
description: "mainブランチとの指定のブランチの差分をチェックして、結果をHTMLで出力"
argument-hint: "[ branchName ]"
---

# 作業フロー
## 1.リポジトリの差分チェック
- リポジトリのURLはプロジェクトのフォルダの設定を取得
- mainブランチが見つからない場合、他のブランチを探して確認する
- mainブランチとブランチ$ARGUMENTの差分をチェックし、HTMLで結果を出力
- 左半分をmainブランチの表示、右半分をチェックするブランチのコードの差分として表示するスタイルで作成
- 差分の文字だけ強調表示
- 作成フォルダは以下の命名規則に従い作成し、.aiDocsが存在しない場合は作成する

### 作成ディレクトリ、ファイルの命名規則

```
.aiDocs/[YYYYMMDD_HHMMSS]/$ARGUMENT_diff.html
```

**例：**

- `.aiDocs/20260901_123456/gitSample_develop_diff.html`

## 2.HTMLのレイアウトチェック
- HTMLのレイアウトを確認し、レイアウトが崩れていたら修正する