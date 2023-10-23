# ChatGPT AutoExpert JP (スタンダード版)

**ライセンス**: [Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)

**実際の使用例**
- [量子力学の基本概念](https://chat.openai.com/share/2788ba18-f8e4-47a4-9ae9-23bcccf4c794)

***

**重要**
GPT-3.5モデル用とGPT-4モデル用のカスタム指示があります。適切なものを利用してください

# 目次
- [使い方](#使い方)
  - [コマンド](#コマンド)
  - [詳細度](#詳細度)
  - [AutoExpertの戦略](#AutoExpertの戦略)
  - [関連情報へのリンク](#関連情報へのリンク)
- [インストール方法(１回のみ)](#インストール方法)

# 使い方
[インストール方法(1回のみ)](#インストール方法)からChatGPTへのカスタム指示を指定すると、回答の質が劇的に向上しているはずです。これは、ChatGPTがあなたの指示文と生成途中の文章を注意しながら文章を作成しているからです。より詳細な内容はDustin Miller氏が書いた[記事](https://spdustin.substack.com/p/whatre-you-lookin-at-chatgpt)(英文)を読むことができます。

## コマンド

| コマンド                          | 説明文                                                                                                                | GPT-3.5 | GPT-4 |
|:---------------------------------|:---------------------------------------------------------------------------------------------------------------------------|---------|-------|
| `/help`                          | スラッシュコマンドの説明を表示します (GPT-4では他の機能も表示します)| ✅       | ✅     |
| `/review`                        | 自分の回答を批判的に評価して、間違いや情報不足を補います| ✅       | ✅     |
| `/summary`                       | 質問を要約して会話の内容から重要な結論を導き出します| ✅       | ✅     |
| `/q`                             | より詳しく質問できる内容を提案してくれます| ✅       | ✅     |
| `/more [話題/見出し(任意)]` |指定した話題などを深掘りします| ✅       | ✅     |
| `/links`                         | 関連性のあるリンクをGoogle Seachから取得します| ✅       | ✅     |
| `/redo`                          | 別の枠組みや方法論を使って、もう一度別の答えを言います| ❌       | ✅     |
| `/alt`                           | 現在の話題について別の見解を言います| ❌       | ✅     |
| `/arg`                           | 現在の話題についてより議論的な見解を言います| ❌       | ✅     |
| `/joke`                          | 現在の話題についての面白い話を言います| ❌       | ✅     |

## 詳細度
質問の前に`V=[1–5]`を付けることで、回答の詳細度を変更することができます。
- `V=1`: 極めて簡潔な内容
- `V=2`: 簡潔な内容
- `V=3`: 詳細な内容(デフォルト)
- `V=4`: 包括的な内容
- `V=5`: 包括的で詳細な内容

## AutoExpertの戦略
ChatGPTは応答の最初に"前書き"を作成するように指示されます。この前書きはChatGPTの "自己注意メカニズム "を自動的に調整し、特定のトークンに注意を向けさせるようにします。この前書きによって、より質の高いアウトプットができるようになります。

- 質問に対する最良の専門家を選択します。これを指定することで、専門家のスタイルとトーンで応答する可能性が高くなります。
- 専門家が通常使用する可能性のある重要なトピック、フレーズ、人物、専門用語を提案します。
これらの "可能性のあるキーワード "は、GPTモデルに、その自己注意メカニズムのための別のアンカーセットを与え、出力の質を向上させます
- ChatGPTのための質問の例として言い換える。これはGPTモデルのための効果的なクエリの書き方にするだけでなく、GPTモデルの自己注意メカニズムをより効果的に活用するために言い換えます。
- 具体的な方法論、フレームワーク、思考プロセスを詳述する。"思考の連鎖"の概要を記述させることで、回答の論理性と一貫性を向上させます


## 関連情報へのリンク
専門家への免責事項などを避け、重要語句への関連リンクを貼るようにします。

**注意** 現時点ではリンク先が英語になってしまっています

## インストール方法
1. [ChatGPT](https://chat.openai.com)にサインインします
2. 左下のアイコンが表示されているプロファイルボタンをクリックして、「カスタム指示」を選択します
3. 必要に応じて、現在のカスタム指示をバックアップしてください
4. 使用しているChatGPTのモデルに応じて"About Me"の内容を最初のテキストボックス内にコピーペーストしてください(現在はGPT-4のみ対応)
  - GPT 3.5: (しばらくお待ち下さい)
  - GPT 4: [`standard-edition/chatgpt_GPT4__about_me.md`](https://raw.githubusercontent.com/roger-sato/ChatGPT-AutoExpert-JP/main/standard-edition/chatgpt_GPT4__about_me.md)
5. 使用しているChatGPTのモデルに応じて"Custom Instructions"の内容を2つ目のテキストボックス内にコピーペーストしてください(現在はGPT-4のみ対応)
  - GPT 3.5: (しばらくお待ち下さい)
  - GPT 4: [`standard-edition/chatgpt_GPT4__custom_instructions.md`](https://raw.githubusercontent.com/roger-sato/ChatGPT-AutoExpert-JP/main/standard-edition/chatgpt_GPT4__custom_instructions.md)
6. 「保存」ボタンをクリックしてください

## ライセンスとクレジット
このプロジェクトは「Dustin Miller」による「ChatGPT-AutoExpert」を基にしていますが、変更が加えられています。この作品は[Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) ライセンスの下に提供されています。

Photo by Dustin Miller, used under [Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/). Modified from original.
