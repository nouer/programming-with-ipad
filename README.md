# iPad Pro(2018) でプログラミングをするための環境

---

<img src="https://raw.githubusercontent.com/nouer/programming-with-ipad/images/images/devenv.png" width="50%">

---

## 目標としたい環境
- Windows, MacからSSH経由でやっていることを、代わりにiPadで。
- 外出先からも。加えて、WindowsをRDPで操作したい。
- 踏み台サーバを経由してのSSH、トネリング経由でのRDP。
- エディタはできたらVimの操作がしたい。
- CodeCommit, GitHubのリポジトリをいじりたい。
- ローカルでもGit操作したい。
- VPN経由でも操作したい。

---

## インストールしたアプリ

### Working Copy
- CodeCommitのリポジトリ操作
- GitHubのリポジトリ操作
> ※ SSHの鍵を暗号化したまま利用できない

### Textastic
- Working Copyと連携してソースコード操作
- Textasticから開くファイルをブラウズして選択することもできる
- Working Copyからファイルを開く（共有）からTextasticを選択して編集もできる
- SSHクライアントも内蔵、SSHの鍵も暗号化したまま利用できる

### iVim
- Working Copyと連携してソースコード操作
- Working Copyからファイルを開く（共有）からiVimを選択して編集する
- 編集はWorking Copyに反映される
> ※ 編集後、Working Copyに戻って内部的にはファイルは変更されているが、差分表示に反映されないことがある。

### Prompt 2
- SSHアクセス（他のSSHクライアントは日本語が不便）
- SSH多段アクセス （ssh agentを利用、ProxyCommandをサポートしているクライアントは見つからなかった）
> ※ SSHトネリング機能は無い

### ~~vSSH~~ ← APP STOREから削除された
- ~~SSHトネリング~~

### Web SSH
- SSHトネリング
> ※ SSHクライアントとしては日本語が不便
> ※ トネリング中、3分間非アクティブだと通知を出してくれてすぐアクティブにできる

### Remote Desktop
- Windowsクライアントアクセス、マイクロソフト謹製
- Web SSHのSSHトネリングでbastionを経由して内部へはアクセス
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

### DrawExpress
- 図形描画ツール、シーケンス図や、ネットワーク図を作成する時に利用

### torguard
- VPNツール、IPを海外からのアクセスとしてテストする際に利用

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

