# 🚀 FC 2025: Upstage DP + LLM + Weave Hands-On

[👉 Fully Connected 2025 Tokyo](https://wandb.ai/site/resources/events/fully-connected/tokyo/) の  **Upstage ハンズオン** 用リポジトリです。


このハンズオンでは、以下の 3 つの技術を組み合わせてドキュメント処理と情報抽出の自動化を実践します。

- 🧾 Upstage Document Parse  
- 🧠 Upstage Solar（LLM）  
- 🧪 Weave（評価・トレース）

## 🧰 環境設定

### 🧪 1. Google Colab の場合
> ⚠️ 現在準備中（TODO）


### 💻 2. Local Jupyter Notebook の場合

#### Python 仮想環境のセットアップ
```sh
# python version : 3.9 / 3.10 で動作確認済

# 1. 仮想環境を作成・有効化
python3.10 -m venv venv_fc_upstage
source venv_fc_upstage/bin/activate  # Mac/Linux
# venv_fc_upstage\Scripts\activate   # Windows

# 2. 依存ライブラリをインストール
pip install -r requirements.txt

# 3. APIキーを設定
export UPSTAGE_API_KEY="YOUR_API_KEY"
export OPENAI_API_KEY="YOUR_API_KEY"

# 4. Jupyter Kernel に登録
python -m ipykernel install --user --name=venv_fc_upstage --display-name "Python (venv_fc_upstage)"

# 5. Notebook 起動
jupyter notebook
```

- Kernel → Python (venv_fc_upstage) を選択

### 🧑‍💻 3. VSCode Notebook の場合
#### 仮想環境のセットアップ
```sh
# python version : 3.9 / 3.10 で動作確認済

# 1. 仮想環境を作成・有効化
python3.10 -m venv venv_fc_upstage
source venv_fc_upstage/bin/activate  # Mac/Linux
# venv_fc_upstage\Scripts\activate   # Windows

# 2. 依存ライブラリをインストール
pip install -r requirements.txt
```
#### .env ファイルの設定
```sh
UPSTAGE_API_KEY="YOUR_API_KEY"
OPENAI_API_KEY="YOUR_API_KEY"
```
#### VSCode の設定
- Extensions → Jupyter Notebook をインストール
- Select Kernel → venv_fc_upstage を選択


## 🔐 UPSTAGE APIキーの取得
- [Upstage API keys](https://console.upstage.ai/api-keys)にアクセスし、APIキーを発行・コピーしてください。
- .env または export コマンドで環境変数として設定します。