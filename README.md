# FC 2025: Upstage DP + LLM + Weave HandsOn

[Fully Connected 2025 Tokyo](https://wandb.ai/site/resources/events/fully-connected/tokyo/)のUpstageハンズオンコード

## 環境設定
### 1. Google Colab利用の場合
TODO

### 2. Local Jupyter Notebook利用の場合

```sh
# python version : 3.9/3.10テスト済

# 1. 仮想環境を作成・有効化
python3.10 -m venv venv_fc_upstage
source venv_fc_upstage/bin/activate  # Mac/Linux
# venv_fc_upstage\Scripts\activate   # Windows

# 2. 
pip install -r requirements.txt

# 3.
export UPSTAGE_API_KEY="YOUR_API_KEY"
export OPENAI_API_KEY="YOUR_API_KEY"

# 4. 
python -m ipykernel install --user --name=venv_fc_upstage --display-name "Python (venv_fc_upstage)"

# 5. 
jupyter notebook
```

- kerner -> Python (venv_fc_upstage)


### 3. Local VSCode Notebook利用の場合
- venv setting
```sh
# python version : 3.9/3.10テスト済

# 1. 仮想環境を作成・有効化
python3.10 -m venv venv_fc_upstage
source venv_fc_upstage/bin/activate  # Mac/Linux
# venv_fc_upstage\Scripts\activate   # Windows

# 2. 
pip install -r requirements.txt
```

- [envファイル](.env)設定
```sh
UPSTAGE_API_KEY="YOUR_API_KEY"
OPENAI_API_KEY="YOUR_API_KEY"
```

- Extentions -> Jupyter Notebook Install

- Select Kernel -> venv_fc_upstage
