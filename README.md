# 🚀 FC 2025: Upstage DP + LLM + Weave Hands-On

[👉 Fully Connected 2025 Tokyo](https://wandb.ai/site/resources/events/fully-connected/tokyo/) の  **Upstage ハンズオン** 用リポジトリです。


このハンズオンでは、以下の 3 つの技術を組み合わせてドキュメント処理と情報抽出の自動化を実践します。

- 🧾 Upstage Document Parse  
- 🧠 Upstage Solar（LLM）  
- 🧪 Weave（評価・トレース）

## 🧰 環境設定

Google Colabの利用をおすすめしますが、
- Local Jupyter Notebook
- VSCode

の利用も可能です。

### 🧪 1. Google Colab の場合

0. [Test Code](https://colab.research.google.com/github/nhandsome-new/fc_2025_upstage_handson/blob/main/Upstage_HandsOn_Test.ipynb)
   - ハンズオン参加の前、事前にご確認ください。
   - Upstage / Weave / 環境の確認
1. [Upstage_HandsOn_1](https://colab.research.google.com/github/nhandsome-new/fc_2025_upstage_handson/blob/main/Upstage_HandsOn_1.ipynb)
   - Upstage Document Parse(DP) / Upstage Solar Pro 2(LLM) の理解・動作確認
   - Upstage Document Parse(DP) / Upstage Solar Pro 2(LLM) の活用例
   - WeaveのTrace機能
2. [Upstage_HandsOn_2](https://colab.research.google.com/github/nhandsome-new/fc_2025_upstage_handson/blob/main/Upstage_HandsOn_2.ipynb)
   - Upstage Document Parse(DP) / Upstage Solar Pro 2(LLM) を用いた、情報抽出
   - 実活用のための修正
3. [Upstage_HandsOn_3](https://colab.research.google.com/github/nhandsome-new/fc_2025_upstage_handson/blob/main/Upstage_HandsOn_3.ipynb)
   - Weaveの評価


#### 参考（ご興味のある方）
- [Option_Upstage_HandsOn_2_All_Results](https://colab.research.google.com/github/nhandsome-new/fc_2025_upstage_handson/blob/main/Upstage_HandsOn_2_All_Results.ipynb)
  - サンプルデータを用いた、情報抽出の結果

- [Option_Upstage_HandsOn_3_Plus](https://colab.research.google.com/github/nhandsome-new/fc_2025_upstage_handson/blob/main/Upstage_HandsOn_3_Plus.ipynb)
  - OPENAI API KEYのお持ちの方
  - OPENAI Embedding Modelを用いた、文字列の類似度評価 

- Upstage PlayGround：UI上、Document Parse（Document AI）・Syn Pro（LLM）が試せます。
  - Jupyter Notebook / Code になれてない方、簡単に他の書類を試してみたい方
  - [Document Parse](https://console.upstage.ai/playground/document-parsing)
  - [Syn Pro](https://console.upstage.ai/playground/chat?model=syn-pro)

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
export WANDB_API_KEY="YOUR_API_KEY"

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
WANDB_API_KEY="YOUR_API_KEY"
```
#### VSCode の設定
- Extensions → Jupyter Notebook をインストール
- Select Kernel → venv_fc_upstage を選択


## 🔐 APIキーの取得
- [Upstage API keys](https://console.upstage.ai/api-keys)・[WANDB](https://wandb.ai/authorize)にアクセスし、APIキーを発行・コピーしてください。
- .env または export コマンドで環境変数として設定します。