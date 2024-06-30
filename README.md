

# **MineCraft-Mod-Translate-Tool**
マインクラフトjava版の一部のMODを以外を翻訳するリソースパックを作成できます。

# 使い方  
Releasesからファイルをダウンロードして任意のフォルダーに配置してください。または自分でコンパイルすることもできます。  
1. ソフトを起動する。
2. 翻訳するMODのバージョンを選択します。
3. 手動でファイルを選択します。もしくは、modsフォルダーのパスをクリップボードにコピーしてボタンをクリックし、**しばらくすると**翻訳が開始されます。
4. 翻訳が完了するまで待ってください。
5. 実行ファイルと同じ階層に translate_rp というフォルダがあるのでマインクラフト内でリソースパックとして読み込ませてください。
6. MODで追加されたアイテムの名前などが翻訳されます。

# 注意点  
- 言語ファイルを持たないMODは翻訳できません。  
- Bedrock版のアドオンなどは翻訳できません。  
- Lunar Client や Bad lion client などのクライアントは翻訳できません。  
- 翻訳したファイルは個人使用にしてください。配布はご遠慮ください。  
- 翻訳時に変数が誤動作を引き起こしてゲーム内での表示が崩れる場合があります。issueにてMOD名とバージョンとともに教えてくださると助かります。  
- 翻訳方法はPythonのgoogletransを採用しています。APIは要求するようにしていないので動作が不安定な場合があるそうです。
- このツールはGoogle翻訳APIを使用しています。そのため、翻訳の品質はGoogle翻訳の結果に依存します。  
- 有料のAPIは必要はありません。Pythonのgoogletrans(4.0.0rc1)による無料の翻訳です。  
- 大量のファイルを一度に翻訳すると、Google翻訳APIの制限に達する可能性があります。その場合、一定時間待つことで再度翻訳を行うことができます。
- 最初のバージョン選択画面に自分の使用したいMODのマインクラフトバージョンがない場合は、ツールに表示されている中で一番新しいバージョンを選択し、ゲーム内でリソースパックとして読み込むときに警告を無視すれば問題なく動作します。  

# 改善点
-  [ ] ~~翻訳元と翻訳先の言語を選択できるようにする~~(有名になったらいずれやる)
-  [ ] MODの中にあるMODが翻訳されない問題(これも有名になったら)
-  [ ] グーグルスプレッドシート等を利用してすでに翻訳したことのあるMODの言語ファイルを呼び出せるようにする(権利問題の可能性？)
-  [ ] 出力されたリソースパックを自動でクリップボードにコピーする(技術的に不可能?)
-  [x] UIの改善
-  [x] tempフォルダを自動作成
-  [x] バージョン未選択時のダイアログ
-  [x] 翻訳完了時の通知~~と通知音の設定~~を追加
-  [x] **並列処理による複数MODの同時翻訳**
