# こうかとんのスカイフラッグ

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
敵に卵を投げ、倒しながら、旗を５本速く取るゲーム

## ゲームの遊び方
* 矢印キーでこうかとんを操作し，出てくる敵をスペースキーで出てくる卵で倒す
* 旗を５本取ったらクリア
* チキンを食べるとライフが１増える
* １から５を押すとレベルが変わり、スピードが変わる
* ライフが０になったら、ゲームオーバーとなる

## ゲームの実装
### 共通基本機能
* 背景画像（動く）と主人公キャラクターの描画　タイム表示　スコアも作る

### 担当追加機能
* ゲームオーバー画面とクリア画面（担当：敵担当、旗担当）：敵とぶつかったときに表示させる　旗を5本とったら表示する
* 攻撃をする（担当：山崎）：主人公は卵を投げて敵に攻撃をする
* チキンを食べる（担当：加藤）：適当なタイミングで一回表示　食べたら少し大きくなりライフが１増える　ライフ表示
* 敵を作る（担当：中島）：敵を右からランダムに表示させる　倒したらスコアが増える
* 旗を作る（担当：佐伯）：ランダムで旗を表示させる　5本取ったらクリア
* 難易度を作る（担当：坪井）：難易度を1から5まで作る　１を押すとレベル１、５を押すとレベル５　レベル表示

### ToDo
- [ ] 当たり判定を大きくする
- [ ] 画面外に出たらself.killする（エラーが出て実装できず）