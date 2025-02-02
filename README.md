# AI-command-samples

それぞれのAIサービスのAPIを叩いて、コマンドラインから利用するコマンドです。

コマンドラインで読みやすいように、返す答えはできるだけシンプルで短い内容にしています。（詳細はプロンプトを御覧ください）

各コマンドは、それぞれの生成AIが生成したスクリプトを多少修正したものです。（自力ででエラーが解決できなかったため。）

各コマンドは、呼び出された端末セッションが継続する限り、質問と答えの内容を保持します。

例）

```bash
$> gemini 梨と洋梨の違いは？
主に果肉の硬さと甘さ、そして形と大きさです。梨はシャキシャキとした硬めの果肉で、洋梨は柔らかくジューシーです。洋梨の方が甘みが強く、形は洋梨のように丸みを帯びています。
(10:58:57) ○ [hiro@hiro-laptop] /mnt/c/Users/hirok/OneDrive/デスクトップ
$> gemini 値段の違いは？
一般的に、洋梨の方が梨より高いです。
```

--showオプションで、セッションで保持している質問と答えを表示します。

--clearオプションで、セッションで保持している質問と答えを削除します。

足りない機能は、このスクリプトを喰わせて、生成AIへ指示すれば、作ってくれるでしょう。

## 要件

curlコマンドとjpコマンドを内部で使用しています。用意してください。

## 使用法

使用する前にAIサービスのAPIキーを取得する必要があります。サービスにより、有償であったり、プリペイドであったりします。

各スクリプトを読んでもらえば、APIキーを設定する環境変数はわかります。事前に設定してください。利用するモデルを指定する必要があるものもあります。