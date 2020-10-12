# pipenvSample
Pipenv説明用のサンプルプロジェクトです。
サンプルのpipfileはpython3.8とpandasがインストールされます。

<br/>

## Pipenvについて
PipenvはPythonが推薦する依存関係管理ツールです。
Node.jsで言うところのpackage.jsonをもとにnpmでモジュールをインストールするようなものです。

<br/>

## 前提
Python実行環境

<br/>

## インストール方法
Pipenv をインストールする場合は以下のコマンドです。
```
pip install pipenv 
```

<br/>

## Pipfileの作成
Pythonプロジェクトのフォルダ内にPipfileがない場合、以下のコマンドで自動でPipfileが作成されます。

<br/>

**Pythonの仮想環境の構築を行う場合**

```
pipenv install --python {バージョン}
```

**モジュール(ライブラリ)をインストールする場合**
```
pipenv install {モジュール名}
```

その際、PipfileとPipfile.lockという2つのファイルが作成されます。
pipfile.lockは、インストールしたパッケージが依存しているパッケージとそのバージョンを管理したり、パッケージの改ざんを防ぐためのものです。


<br/>

## Pipfileからインストール
Pythonプロジェクトのフォルダ内にPipfileがある場合、以下のコマンドでPipfileに書かれた環境やモジュールがインストールされます。

```
pipenv install
```

<br/>

## モジュールのアンインストール
インストールしたモジュールを削除する場合は以下のコマンドです。

```
pipenv uninstall {モジュール名}
```

<br/>

## その他
仮想環境内でコマンドを実行するrunコマンドやPipfileの内容をPipfile.lockへ反映するlockコマンド等があります。
