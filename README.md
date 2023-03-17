## システムの構築方法（ナレッジグラフ推論チャレンジ用）
### 事前に準備すること
1. Anaconda（実行環境はAnaconda）
2. Anaconda で仮想環境構築
3. jupyter のインストール
4. [VirtualHome2KG](https://github.com/aistairc/VirtualHome2KG) のセットアップ
5. virtualhome2kg/demo/unity_demo.ipynb が正常に動かせることを確認（VirtualHome自体が動かせることを確認）

## 本システムの実行準備
1. VirtualHomeが動くことが確認出来たら，本システムgenerate_action_scriptsを，virtualHome2kg以下に置く
2. virtualhome2kg/generate_action_scrips以下で，pip install -r requirements.txt を実行
3. python -m spacy download en_core_web_sm を実行

## 本提案システムの実行方法
2. virtualhome2kg/simulation/unity_simulator/VirtualHome.exe を実行
3. Anaconda Pronpt で，jupyter notebook を実行
4. jupyter notebook 上で，generate_action_script.ipynb を開く
5. 画面右上の"Logout"の下に，Python の環境が表示されるので確認
6. Python 環境が，(environment name)ではない場合，Kernelから，Change kernelを選択し，Python 環境を，(environment name)に変更
7. Python 環境が，(environment name)に変更されたか確認
8. 上から順に実行していき，最後のセルに，行動のラベル，行動の説明文を入力する箇所があるので，入力をして実行する．
9. generate_action_scrips/output 以下に，アクションスクリプトが生成される
