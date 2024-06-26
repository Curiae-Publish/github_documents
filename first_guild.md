
# 1. アカウント作成するサイト

- Google
- GitHub

## 1.1. Google

- Google Driveでデータを共有することがあるので、Web部署のメンバーに共有できるGoogleアカウントを用意しておくこと

## 1.2. GitHub

### 1.2.1. アカウント作成

すでにアカウントがある人は飛ばしてください

- <a href="https://github.com/" target="_blank" rel="noopener noreferrer">GitHub</a>にアクセスし、「Email address」にメールアドレスを入れ「Sign up for GitHub」をクリックする

> [!NOTE]  
> 大学のではなく、**個人のメールアドレス**で登録してください  
> また、メールアドレスは設定しない限り公開されません

- 遷移後のページで「Continue」
- パスワードを入力し「Continue」
- ユーザーネームを入力し「Continue」

> [!NOTE]  
> ユーザーネームは本名である必要はなく、全世界に公開されることを想定したものにしてください  
> （SNSアカウントと同名にするのも良いです）

- メールが送られてくるので、コードを入力してアカウント作成を終える
- 必要に応じて再度ログインをし、「Dashboard」と書かれたページに行けばアカウント作成は完了

### 1.2.2. アカウント設定

- 右上のアイコンのようなものをクリックして「Your Profile」へ飛ぶ
- 「Edit Profile」から適当に設定をしてください

> [!NOTE]  
> 初期設定のままでもいいですが、アイコンなどを変更したほうが識別しやすいです

---

# 2. インストールするアプリケーション

- Visual Studio Code (VSCode)
- Git

## 2.1. VSCode

ダウンロードしている人はスキップして構いません

### 2.1.1. インストール

- <a href="https://code.visualstudio.com/download" target="_blank" rel="noopener noreferrer">ダウンロードリンク</a>から対応するOSでインストールする
- 特にこだわりがなければ、青いボックスのを選択すればよい
- ダウンロードしたインストーラを実行する
- 基本的には「次へ」を選択すればよいが、必要に応じて「デスクトップ上にアイコンを作成する」を選択する

### 2.1.2. 環境設定

- VSCodeを起動し、![Extension](images/extension.png)を選択する
- 検索欄を用いて、「Japanse Language Pack for Visual Studio Code」をInstallする
- インストールが終了すると画面右下に「Change Language and Restart」と出るのでクリックする（再起動）
- 表示が日本語化されれば初期設定は終了

## 2.2. Git

VSCodeの画面上部のタブから「ターミナル」>「新しいターミナル」を選択して

```bash
git --version
```

を実行してください

実行後、

```bash
git version 2.43.0.windows.1
```

のようなメッセージが返ってこない場合は、Gitがインストールされていません  
下記の手順を行ってください

### 2.2.1. インストール

- <a href="https://gitforwindows.org/" target="_blank" rel="noopener noreferrer">ダウンロードリンク</a>から「Download」をクリックする
- ダウンロードしたインストーラを実行する
- 「Choosing the default editor used by git」まで「Next」をクリックする
- 「Use Visual Studio Code as Git's default editor」を選択し「Next」
- 「Let Git decide」を選択し「Next」
- 「Git from the command line and also from 3rd-party software」を選択し「Next」
- 「Use bundled OpenSSL」を選択し「Next」
- 「Use the OpenSSL library」を選択し「Next」
- 「Checkout Windows-style, commit Unix-style line endings」を選択し「Next」
- 「Use MinTTY (the default terminal of MSYS2)」を選択し「Next」
- 「fast-forward or merge」を選択し「Next」
- 「Git Credential Manager」を選択し「Next」
- そのまま「Next」して、なにもチェックせずに「Install」
- 「Completing the Git Setup Wizard」と表示されれば終了

> [!NOTE]
> ある項目がスキップされて次の項目が出てくる場合があります  
> そのときは、出てこなかった項目をスキップして進めてください  

### 2.2.2. 環境設定

- VSCodeを再起動してインストールされているか確認

    ```bash
    git --version
    ```

    を実行して

    ```bash
    git version 2.43.0.windows.1
    ```

    が帰ってくればOK

- インストールされている場合は初期設定を行う
- ユーザー名はGitHubと同じものを推奨

```bash
git config --global user.name "User Name"
```

- メールは<a href="https://github.com/settings/emails" target="_blank" rel="noopener noreferrer">GitHubの設定</a>から見れる`123456789+username@users.noreply.github.com`という形式を使用することをおすすめする

```bash
git config --global user.email "Email Address"
```

> [!WARNING]  
> ここで設定した情報はすべて公開されます

- 以上でGitの初期設定は終了

---

前提となる環境構築はおしまいです。  
おつかれさまでした🥰

> ref.
>
> - [Windows への Visual Studio Code のインストール方法](https://www602.math.ryukoku.ac.jp/Prog1/vscode-win.html)
> - [Gitのインストール方法(Windows版)](https://qiita.com/T-H9703EnAc/items/4fbe6593d42f9a844b1c)
