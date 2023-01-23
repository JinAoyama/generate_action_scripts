# generate_action_scripts

## 本提案システムの構築方法
### Anaconda
1. Anaconda のインストール
2. Anaconda Pronpt を起動

#### 仮想環境構築
3. conda env create -n (environment name)
4. conda activate (environment name)
5. pip install -r requirements.txt を実行

※(environment name) には任意の名前を入力

### VirtualHome2KG
6. [VirtualHome2KG](https://github.com/aistairc/VirtualHome2KG)のダウンロード
7. [VirtualHome2KG](https://github.com/aistairc/VirtualHome2KG)を参考にして，セットアップ
8. 本システムのフォルダ，generate_action_scripts を，virtualHome2kg 以下に置く
9. cdコマンドで，virtualhome2kg/generate_action_scrips まで移動

## 本提案システムの実行方法
1. virtualhome2kg/simulation/unity_simulator/VirtualHome.exe を実行
2. Anaconda Pronpt で，jupyter notebook を実行
3. generate_action_script.ipynb を開く
4. jupyter notebook が開くので，画面右上の"Logout"の下に，Python の環境が表示される．
5. Python 環境が，(environment name)ではない場合，Kernelタブから，Change kernelを選択し，Python 環境を，(environment name)に変更
6. Python 環境が，(environment name)に変更されたか確認
7. 上から順に実行していき，最後のセルに，行動のラベル，行動の説明文を入力する箇所があるので，入力をして実行する．
8. generate_action_scrips/output 以下に，アクションスクリプトが生成される
