# Machine_Learning
## 本リポジトリの概要
- 本リポジトリでは、機械学習講座を準備するにあたって躓いたポイントの記録や機械学習講座で使用するノードブックを管理する
## MinicondaとPythonのインストール
### 参考にした記事
- [Qiita](https://qiita.com/c60evaporator/items/b6a7394231d1e768ce64#miniforge%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB)
### Miniconda
- Minicondaは、インタプリタ切替＆パッケージ切替用のツール
- Anaconadaは商用有料化に引っかかるので今回は使用しない<br>
([公式：PURCHASED VS. FREE OFFERINGS](https://legal.anaconda.com/policies/en/#terms-of-service))
#### インストール
- [Minicondaのインストーラー](https://docs.conda.io/en/latest/miniconda.html#windows-installers)から、Windows用の`Miniconda3 Windows 64-bit`(Latest version)をインストールする。
- 基本的にNextをクリックするが、「Advanced Installation OptionsConda」では「Register Miniforge3 as my default Python 3.10」にチェックする。
- 最後のInstallをクリックする
- インストールが終わったら、Windowsの検索画面でAnacondaと打ち込むと、Anaconda Prompt(miniconda3)が出てくるので開く。
#### パッケージレジストリの変更
- Pythonの各種パッケージを管理しているレジストリのこと。デフォルトはAnacondaとなっているので、無料のconda-forgeに切り替える。
- まず、以下のコマンドで現在のリポジトリを確認する。
```conda config --show channels```<br>
