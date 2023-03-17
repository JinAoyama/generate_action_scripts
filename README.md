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
1. virtualhome2kg/simulation/unity_simulator/VirtualHome.exe を実行
2. Anaconda Pronpt で，jupyter notebook を実行
3. jupyter notebook 上で，generate_action_script.ipynb を開く
4. 上から順に実行していき，最後から2番目のセルでデータセットからアクションスクリプト生成
5. 最後のセルでは，データセットとは他のデータ，行動のラベル，生活行動を表現する自然言語文を入力して実行するとアクションスクリプトが生成される．
6. アクションスクリプトはgenerate_action_scrips/output 以下に生成される.最後から３番目のセルで生成する場所を指定している．