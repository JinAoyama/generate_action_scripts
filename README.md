## 本提案システムの構築方法
### Anaconda
1. Anaconda のインストール
2. Anaconda Pronpt を起動

#### 仮想環境構築
3. conda env create -n (environment name)
4. conda activate (environment name)

※(environment name) には任意の名前を入力

### VirtualHome2KG
5. [VirtualHome2KG](https://github.com/aistairc/VirtualHome2KG)のダウンロード
6. [VirtualHome2KG](https://github.com/aistairc/VirtualHome2KG)を参考にして，セットアップ

### generate action scripts
7. 本システムのフォルダ，generate_action_scripts を，virtualHome2kg 以下に置く
8. virtualhome2kg/generate_action_scrips まで移動
9. pip install -r requirements.txt を実行
10. python -m spacy download en_core_web_sm を実行

## 本提案システムの実行方法
1. virtualhome2kg/generate_action_scrips まで移動
2. virtualhome2kg/simulation/unity_simulator/VirtualHome.exe を実行
3. Anaconda Pronpt で，jupyter notebook を実行
4. generate_action_script.ipynb を開く
5. jupyter notebook が開くので，画面右上の"Logout"の下に，Python の環境が表示される．
6. Python 環境が，(environment name)ではない場合，Kernelから，Change kernelを選択し，Python 環境を，(environment name)に変更
7. Python 環境が，(environment name)に変更されたか確認
8. 上から順に実行していき，最後のセルに，行動のラベル，行動の説明文を入力する箇所があるので，入力をして実行する．
9. generate_action_scrips/output 以下に，アクションスクリプトが生成される
