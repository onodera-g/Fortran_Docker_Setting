
# Fortran_Docker_Setting
このリポジトリでは、VsCode、Docker、gfortran を使用して Fortran の実行環境の構築することができます。

本環境を構築することにより、静的コード解析、ソースコードの自動整形、シンタックスハイライト、入力補完、等を利用することができます。

また、OSに依存せず同じ手順で環境を構築することができます。

<!--# DEMO
プログラムの作成、プログラムの作成、コンパイル、デバッグの方法を載せた動画を記載
-->

# Features
* Dockeを用いて仮想環境上にFortranの実行環境を構築するため、OSに依存せず同じ手順で環境を構築することができます。
* VsCodeの拡張機能を利用することで、静的コード解析、ソースコードの自動整形、シンタックスハイライト、入力補完を利用することができます。

# Requirement
* Docker
* Visual Studio Code
* gfortran

# Installation
### 1. Docker Desktopのインストール
https://www.docker.com/ja-jp/products/docker-desktop/


### ２. VScodeのインストール
https://code.visualstudio.com/Download


### 3. Vscode拡張機能のインストールする。
Vsccodeのアクティビティーバーから、以下の拡張機能をインストールします。
>1. Docker
>2. Remote Development
>3. Japanese Language Pack for Visual Studio Code


### ４. 作業フォルダを作成、設定ファイルの保存
作業フォルダを作成します。作成したフォルダはFortranのプログラムを格納する場所になります。作成場所はどこでも問題ありません。

次に本リポジトリをダウンロードし、先ほどの作業フォルダに保存します。保存場所は作業フォルダのルートディレクトリとします。


### ５. Dockerコンテナの作成
Fortranの実行環境をインストールします。実行環境のインストールは以下の手順で行います。

>1. ステータスバーから「リモートウィンドウ」を開く。
>2. コンテナーでフォルダを開く」を選択する。開くフォルダは、「4.1 作業フォルダの作成」で作成したフォルダを指定します。
>3. 実行環境のインストールが始まりますので待ちます。**インターネット環境が必要になります。**

![スクリーンショット 2024-05-26 16.09.53.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3259514/102bf6a1-8117-b20b-7097-81bef8c43820.png)

![スクリーンショット 2024-05-26 16.56.27.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3259514/7fda17ad-4dd8-4d6a-786d-398ea64ad401.png)



# Usage
作業フォルダ内に保存されてある**test.f95**を例に、使い方を説明します。

>1. 「サイドバー」にあるファイルを選択することで、「エディター」にファイルを表示します。
>2. 「上書き保存(Command+S)」することで、静的コード解析、リファクタリングが行われます。
>2. 「Shift+Command+B」でコンパイルを行います。
>3. 「エディター」の数字の行番番号をクリックすることで、任意の箇所のブレークポイントを設定できます。
>4. 「F5」でプログラムを実行します。
>5. ブレークポイントを設定している場合には、「アクティビティーバー」の「実行とデバッグ」から、プログラム実行中の各変数の値を見ることができます。

<!--<ここに使い方の動画URL>
-->

# Note
動作環境
|PC|OS|CPU|
|--|--|---|
|MacBook Air 2020|macOS Sonoma 14.5|M1|


# License
"Fortran_Docker_Setting" is under [GPL-3.0 license](https://ja.wikipedia.org/wiki/GNU_General_Public_License).
