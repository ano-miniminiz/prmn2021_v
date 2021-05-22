author: ano-miniminiz
summary: GitHubを使うための準備
id: githandson-1
categories: codelab,markdown
environments: Web
status: Published
feedback link: https://github.com/ano-miniminiz/prmn2021_vsc
<!-- analytics account: -->

# GitHubを使いたい！
## はじめに

課題の進捗を確認・共有するために、GitHubというサービスを使用します。
(GitHubについてはググってください)

構造がややこしいため使い慣れるまで少し難しく感じるかもしれませんが、コマンドを数個覚えれば、なんとか使えます。[Gitはじめの一歩](https://www.slideshare.net/ihcomega/git-57454868)を覗いてみるのもアリです。

ただ、少し前にニュースになったように、正しく設定をして使わないと、他人に見られるべきではない情報が大公開されてしまいますので、お気をつけください。


## Gitインストール(Windowsのみ)
WindowsPCを使っている人向けです。MacPCの方はターミナルで`git --version`と入力して、バージョンが表示されることを確認したら、3番に飛んでください。

Positive
: インストールまでの各項目に書かれていることを確認したい場合は[こちら](https://www.curict.com/item/60/60bfe0e.html)を参考にしてください。

[https://gitforwindows.org/](https://gitforwindows.org/) にアクセスする

![git for windows](./figure/ss1.png)
"Download"をクリックしてGitをインストールする

<br>

![explorer](./figure/ss2.png)
エクスプローラを開き、ダウンロードしたインストーラ(.exe)を起動する

<br>

![Information](./figure/ss3.png)
[Next]をクリック

<br>

![Select Components](./figure/ss4.png)
画像と同じ項目にチェックが入っていることを確認して[Next]

<br>

![Choosing the default editor used by Git](./figure/ss5.png)
デフォルトのまま[Next]

<br>

![Adjusting the name of the initial branch in new repositories](./figure/ss6.png)
Let Git decide を選択して[Next]

<br>

![Adjusting your PATH environment](./figure/ss7.png)
2つ目のGit from the ~を選択して[Next]

<br>

![Choosing HTTPS transport backend](./figure/ss8.png)
Use the OpenSSL libraryを選択して[Next]

<br>

![Configuring the line ending conversions](./figure/ss9.png)
3つ目にチェックを入れて[Next]

<br>

![Configuring the terminal emulator to use with Git Bash](./figure/ss10.png)
Use MinTTYを選択して[Next]

<br>

![Choose the default behavior of git pull](./figure/ss11.png)
Defaultを選択して[Next]

<br>

![Choose a credential helper](./figure/ss12.png)
Git Credential Manager Coreを選択して[Next]

<br>

![Configuring extra options](./figure/ss13.png)
デフォルトのまま[Next]

<br>

![Configuring experimental options](./figure/ss14.png)
何も選択せずに[Install]

<br>

![Installing](./figure/ss15.png)
割とすぐ終わります

<br>

![Completing the Git Setup Wizard](./figure/ss16.png)
インストールが終わったら、[finish]をクリックして閉じる

<br>
<br>

### コマンドプロンプトを起動して、Gitがインストールされていることを確認します
<br>

`git --version`と打ってEnter

![Comand prompt](./figure/ss17.png)
バージョンが表示されたらOKです


## リモートリポジトリの作成

GitHubのアカウントは作成済みという前提で説明していきます
(まだの方は[こちら](https://github.com/)からどうぞ)

まずはリモートリポジトリ(GitHub上での管理フォルダ的なもの)を作成します

![New](./figure/ss20.png)
Repositoriesに移動して、右上の[New]をクリック

<br>

以下のような画面が出てくるはずです。
![Create a new repository](./figure/ss21.png)
・Owner:自分のユーザ名

・Repository name:リモートリポジトリの名前(図では`git-test`)

・Public/Private:リポジトリの公開範囲(適宜)

・Add系:必要に応じてチェック、後で追加できます

それぞれ設定が終わったら、[Create repository]をクリックしてリポジトリを作成します

<br>

![Create a new repository](./figure/ss22.png)
後ほど使うのでこのページは開いておくことをおすすめします


## ローカルリポジトリの作成

お次はローカルリポジトリを作成します


