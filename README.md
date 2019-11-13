# NeodymiumProject
磁石をモチーフにしたなんかこう面白そうなゲーム

## 開発環境
|アプリケーション|バージョン|
|:---------------|:---------|
|Unity|2019.2.12f1|
|VisualStudio Community|2019|

## コーディング規約
### StyleCop必須
- コミッターはPR作成時に、
レビュアーはPRチェック時にそれぞれ実行して問題がないか確認を行ってください。
C#7な機能を使用する場合はStyleCop自体がサポートをしていない為
Suppressにするかauto-genなコード扱いにしそのファイルのチェックを無視するようにしてください
導入方法は下記記事を参考にしてください
https://qiita.com/github129/items/8270dc74599e71af5285

### UTF-8 with BOM
- 文字コードは原則BOM付きUTF-8としてください。
EditorConfigを使用しているため最新のVisualStudioを使用していれば問題ないはずです。
別の文字コードになっていた場合は逐次変換を行ってください。

### CRLF
- 改行コードは原則CRLFとしてください。

### その他
- その他ルールはMicrosoft Coding Standardsに準拠してください
https://docs.microsoft.com/ja-jp/dotnet/csharp/programming-guide/inside-a-program/coding-conventions

### 使用可能な文法に関して
- 基本最新言語仕様のものまで使用して問題ありません
トリッキーなコードに関しては可読性を加味してPR時に決めてください。
省略可能な記法がある場合は優先的に使用してください（自動実装プロパティやラムダ式等）
- LINQは積極的に使用してください
- 可能な限り疎結合を意識したコーディングを行ってください
	- 上記に関してステップ数で測ってはいけませんが目安として1メソッド100ステップを超えた場合は切り出しを考えてください
- 楽しくコーディングしましょう

## ツールに関して
- 基本ツールとしてUnity2019 + VisualStudio 2019をベースとします
- 追加のツールとしてVisualStudio Codeがあると便利です
- Gitクライアントは特に指定はありませんがSourceTreeがおすすめです
- 仕様の策定ツールとして最終出力はExcelではなくGoogleSpreadsheetを用います