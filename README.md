# iPad Pro(2018) でプログラミングをするための環境

### Working Copy
- CodeCommitのリポジトリ操作
- GitHubのリポジトリ操作
> ※ SSHの鍵を暗号化したまま利用できない

### Textastic
- Working Copyと連携してソースコード操作
- SSHクライアントも内蔵、SSHの鍵も暗号化したまま利用できる

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

### ProCreate
- 絵画ツール、写真加工を含めて、ペンではやりきれない時に利用

### Phonto
- 画像への文字入れツール、多彩なフォントがある

---


# 見送ったアプリ
### Termius （月額で高杉）
