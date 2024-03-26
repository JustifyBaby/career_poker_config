# career_poker_config

## https://boku-boardgame.net/cards/daifugou-local-rule/
を参考にして、大富豪のローカルルールを整理しました。
## How to use?
* ### 無効にするときは、falseを入力します。
* ### playingでは、有効にする場合、有効にさせるカードの番号を入れます。
* ### 絵柄は、"picture": number;を加えます。
* ### 枚数は、"sheets": string;を加えます。
* ### 依存関係は、"depend": boolean;を加えます。

* ## The keys mean
* igniter: 何のカードで始めるか？
* storngest: 一番強いカード
* poorest: 一番弱いカード
* sandstorm: 砂嵐の有無(有効の時は、sheetsが必要。)
* kill_joker: スぺ３返しの有無(有効の時は、pictureが必要。)
* cut_block: 4止めの有無(有効の時は、sheetsが必要。)
* skip: skipの有無
* omen: オーメンの有無
* hand_over: 7渡しの有無(有効の時は、dependが必要。)
* lucky: ラッキーセブンの有無(有効の時は、sheetsが必要。)
* cut: ろくろ首、八切り、救急車の有無(ろくろ首および救急車が有効の時は、sheetsが必要)
* reverse: ９リバースの有無(有効の時は、dependが必要。)
* rebellion: クーデターの有無
* throw: 10捨ての有無(有効の時は、dependが必要。)
* power_back: 11バックの有無
* bomb: Qボンバーの有無(有効の時は、dependが必要。)
* bind: 縛り
* bind -same: 同じ数の縛り(有効の時は、[true, 枚数]と指定)
* bind -step: 階段縛り(有効の時は、[true, 枚数]と指定)
* down_number: ダウンナンバーの有無
* emperor: エンペラーの有無
* revolution: 革命の有無
* big_revolution: 大革命の有無(有効の時は、[true, トランプの数字]と指定)
* banned: 禁止上がり(有効の時は、[true, 禁止のトランプ]と指定)
* millionaire_fall: 都落ちの有無
* change_cards: カード交換の有無
* ascension: 下剋上の有無
* disaster: 天変地異の有無

## Why Great?
* ### jsonで管理できます。
* ### 有効無効だけでなく、ルールを適用させる絵柄や枚数も設定できます。