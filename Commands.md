# しりとりBot コマンド

## 標準コマンド

### help

コマンドを一覧する。形式自由。

### config set [key] [val] / config clear [key]

Value type の設定に書き込む / 設定から削除する。

config set の [val] は省略可能。省略した場合、現在の設定値を返す。

### config add [list] [key] [val] / config remove [list] [key] / config clear [list]

List type の設定に追加する / 設定から削除する / 全削除する。

### start

既出語をすべて削除して、新しいセッションをスタートする。

## 拡張コマンド

### ranking

現在のユーザーランキングを表示する。

## 設定 key

list / value の判断は、実装上ではなく、ユーザーからどう見えるかで行っています

| key | 種別 | type | val | note |
|:----|:-----|:----|:-----|:-----|
| reply | 標準 | value | on / off | チャンネルへの反応を on / off する |
| minimum-char | 拡張 | value | number | 最短文字列を設定する |
