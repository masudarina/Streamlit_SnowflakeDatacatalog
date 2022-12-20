
# Snowflake データカタログ

## 概要
Snowflake データカタログは、Snowflakeのデータを収集し可視化するツールです。

## 前提条件
・Streamlit Cloud が使用できること

　アカウント作成ページ：https://share.streamlit.io/signup

・Git Hub アカウントを所持していること

　アカウント作成ページ：https://www.winschool.jp/download/online/text/guide_regist_github.pdf

・Git Hub に専用のリポジトリが存在すること

　参考サイト：https://docs.github.com/ja/get-started/quickstart/create-a-repo

・Git Hub 専用のリポジトリが「PUBLIC」設定になっていること

　参考サイト：https://yu-report.com/entry/githubprivate/

## 設定手順
・Git Hub 設定手順

	1. 上記リポジトリ内のファイルをすべてダウンロードする
	

	2. 専用のリポジトリに以下のファイルを配置する

		配置するファイル：
		・Datacatalog.py
		・Snowflake.png
		・requirements.txt

		配置後のディレクトリ構成図の例：
		<リポジトリ名>/
		　├ Datacatalog.py
		　├ Snowflake.png
		　└ requirements.txt

	3. 専用のリポジトリに「.streamlit」フォルダを作成する
	参考サイト：
	https://yoshitaku-jp.hatenablog.com/entry/2018/07/07/225642

	4. 「.streamlit」フォルダに以下のファイルを配置する

		配置するファイル：
		・config.toml

		配置後のディレクトリ構成図の例：
		<リポジトリ名>/
		　├ Datacatalog.py
		　├ Snowflake.png
		　├ .streamlit/
		　│　└ config.toml
		　└ requirements.txt

・Streamlit Cloud アプリデプロイ設定手順

	1. Streamlit Cloud アプリ作成画面の「New app」をクリックする

	2. 「Paste GitHub URL」をクリックする

	3. 専用のGit HubのpythonファイルのURLを貼り、「Deploy!」をクリックする
	URL例：
	https://github.com/masudarina/streamlit/blob/main/Datacatalog.py

・Streamlit Cloud アプリ共有設定手順

	1. Streamlit Cloud アプリ作成画面を開き、共有したいアプリの３点リーダーをクリックする

	2. 「Settings」＞「Sharing」をクリックする

	2. 「Invite viewers by email」に閲覧者のメールアドレスを記入し、「Save」をクリックする
	参考サイト：
	https://docs.streamlit.io/streamlit-cloud/get-started/share-your-app


## 使用手順

1. Streamitからの招待メールを開き、「Accept invite and visit app」を押下する

	参考サイト：
	https://docs.streamlit.io/streamlit-cloud/get-started/share-your-app

2. Webブラウザ画面表示後、Snowflakeの認証情報を入力して「OK」ボタンを押下する

	※Snowflake認証情報は以下を参考に入力する

	アカウント名(必須) : Snowflakeのアカウント名
	ユーザー名(必須) ： Snowflakeアカウント接続時のユーザー名
	パスワード(必須) : ユーザーのパスワード
	ロール : ユーザーにデフォルトのロールが設定されていない場合は、使用するロールを記入
	ウェアハウス : ユーザーにデフォルトのロールが設定されていない場合は、使用するロールを記入

	※ツール確認用URL：
	https://masudarina-st-snowflake-checkwarehousestool-v20220729-01-qam7kk.streamlitapp.com/


新規作成　2022/12/19

