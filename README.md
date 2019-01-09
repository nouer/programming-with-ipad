# iPad Pro(2018) でプログラミングをするための環境

---

<img src="https://raw.githubusercontent.com/nouer/programming-with-ipad/images/images/devenv.png" width="50%">

---

## 目標としたい環境
- Windows, MacからSSH経由のオペレーションを代わりにiPadで。
- 外出先からも。加えて、WindowsをRDPで操作したい。
- 踏み台サーバを経由してのSSH、トネリング経由でのRDP。
- SSHへのアクセスは秘密鍵での認証。できたら秘密鍵もパスフレーズで暗号化しておきたい。
- エディタはできたらVimの操作がしたい。普段はプレーンなVimかVSCodeを利用。
- CodeCommit, GitHubのリポジトリを触りたい。
- ローカルでもGit操作したい。

---

## インストールしたアプリ

### <a href="https://itunes.apple.com/jp/app/working-copy/id896694807?mt=8">Working Copy</a>
- CodeCommitのリポジトリ操作
- GitHubのリポジトリ操作
- エディタと連携しなくても、Working Copy自体のエディタも優れている
- Markdownもプレビュー表示できる
> ※ CodeCommitに利用するSSHの鍵を暗号化したまま利用できない

### <a href="https://itunes.apple.com/jp/app/textastic-code-editor-7/id1049254261?mt=8">Textatic</a>
- Working Copyから連携してファイル編集
- Textasticから開くファイルをブラウズして選択することもできる
- Working Copyからファイルを開く（共有）からTextasticを選択して編集もできる
- SSHクライアントも内蔵、SSHの鍵も暗号化したまま利用できる、SFTPも利用できる
- iOSのブラウズの機能から、Dropbox、GDrive、WorkDocsを始め、様々なオンラインストレージを直接利用できる
- ファイルエンコーディング、改行コードなども操作できる
- Markdownもプレビュー表示できる

### <a href="https://itunes.apple.com/jp/app/ivim/id1266544660?mt=8">iVim</a>
- Working Copyから連携してファイル編集
- Working Copyからファイルを開く（共有）からiVimを選択して編集する
- 編集はWorking Copyに反映される
> ※ 編集後、Working Copyに戻って内部的にはファイルは変更されているが、差分表示に反映されないことがある。

### <a href="https://itunes.apple.com/jp/app/prompt-2/id917437289?mt=8">Prompt 2</a>
- SSHアクセス（他のSSHクライアントは日本語が不便）
- SSH多段アクセス （ssh agentを利用、ProxyCommandをサポートしているクライアントは見つからなかった）
> ※ SSHトネリング機能は無い

### ~~vSSH~~ ← APP STOREから削除された
- ~~SSHトネリング~~

### <a href="https://itunes.apple.com/jp/app/webssh-pro/id497714887?mt=8">WebSSH Pro</a>
- SSHトネリング
> ※ SSHクライアントとしては日本語が不便
> ※ トネリング中、3分間非アクティブだと通知を出してくれてすぐアクティブにできる

### Remote Desktop
- Windowsクライアントアクセス、マイクロソフト謹製
- Web SSHのSSHトネリングで踏台を経由して内部へはアクセス
> ※ 3分に1度、SSHトネリングアクセスしているAPPをアクティブにしないといけない

### JavaScript Anywhere
- JavaScriptの簡単な動作確認

### Node.js for iOS
- Node.jsの環境、自分でビルドして入れる

### MetaMoji Note
- 普段使いのペンでのメモとり、及び、録音

### Whink
- 普段使いのペンでのメモとり、及び、録音（現在はMetaMoji Noteを利用）
> ※ ペンで書きなぐる速度についてこないことが多いので、MetaMoji Noteに変更
> ※ 録音の頭出しは、このアプリが最適

### Procreate
- 絵画ツール、写真加工を含めて、ペンではやりきれない時に利用

### Phonto
- 画像への文字入れツール、多彩なフォントがある

### <a href="https://itunes.apple.com/jp/app/drawexpress-diagram-lite/id687459234?mt=8">DrawExpress</a>
- 図形描画ツール、シーケンス図や、ネットワーク図を作成する時に利用

### <a href="https://itunes.apple.com/jp/app/dash-offline-api-docs/id1239167694?mt=8">Dash</a>
- オフラインでAPIドキュメントを読むための便利ツール

---


# 見送ったアプリ
### Termius
- 月額課金で高杉

### TouchDraw
- 試用版が無いので見送り

### Penultimate
- ペンの反応速度が遅いので不採用

### iTurminal
- 日本語入力がうまくいかなかったので見送り

### SSH Tunnel
- バックグラウンドで動作とあるが、レビュー無いし、試用版無いので見送り

### Coda
- 高杉で試さなかった

---

# 今後、なんとかしたいこと、なったらいいなと思うこと
### SSHのトネリングを利用する時、トネリングをしているアプリがアクティブでないと切断されてしまう。切断されないアプリが欲しい（バックグラウンドで空白の音楽を再生とか？）
### iVimがiOSのブラウズ機能をつかってファイルを開けたらいいのに（:e . からできたらいいのに）
