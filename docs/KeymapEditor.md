# KeymapEditor
一般的なリポジトリをフォークする方法を紹介しますが、「Use this template」から新しいリポジトリを作成することもできます。このリポジトリの内容を引き継ぎつつ、ご自身のプライベートリポジトリとしても使用できます。
## GitHubリポジトリのフォーク  
ファームウェアはGitHub Actionsで書き出します。  
1. GitHubアカウントを持っていない場合は、事前に[アカウント登録](https://github.com/signup)をしてください。  
2. 準備が出来たらこのリポジトリを[フォーク](https://github.com/nazuna293/zmk-Enigma_03-user-config/fork)します。  
<img src="img/FORK_01.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/FORK_02.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/FORK_03.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/FORK_04.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">

## KeymapEditorと連携
キーマップはブラウザ上で編集します。
1. [KeymapEditor](https://nickcoutsos.github.io/keymap-editor/)にGitHubアカウントを連携させます。  
<img src="img/KE_01.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/KE_02.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/KE_03.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/KE_04.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/KE_05.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
2. zmk-config-Enigma_01を連携させます。  
<img src="img/KE_06.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">

4. キーマップを編集します。  
[Behaviors](https://zmk.dev/docs/keymaps/behaviors)や[Keycodes](https://zmk.dev/docs/keymaps/list-of-keycodes)等のドキュメントに詳細が載っています。  
<img src="img/KE_07.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">

5. キーマップを保存します。
<img src="img/KE_09.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/KE_10.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">

## ファームウェアをEnigma_01へ
以下の手順で転送します。
1. GitHub Actionsからファームウェアをダウンロード、解凍します。
<img src="img/KE_11.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">
<img src="img/KE_12.jpg" alt="製品画像" style="width: 100%; max-width: 600px; height: auto;">

2. Enigma_01とパソコンをUSB-Cケーブルで接続します。

3. 本体のリセットボタンを2回押します。  
もしくはキーマップに割り当てたリセットキー(bootloader)を押す


4. フォルダに「XIAO SENSE」が表示されたらファームウェア(Enigma_03.uf2)を貼り付けます。  

## デバイスと再接続  
### 有線接続の場合  
数秒待てば再接続されます。  

### 無線接続の場合  
ペアリング情報がリセットされているので、再ペアリングが必要です。
1. BT_SEL0でメインデバイスとペアリングする
2. BT_SEL1~SEL4でサブデバイスとペアリングする

**BT_CLR_ALL**でペアリング情報をクリアすることもできる
