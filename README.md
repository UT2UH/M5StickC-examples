# M5StickC サンプルスケッチ集

## 概要

ライブラリにするまでもない、細かいスケッチを保存する場所です。

### BLE_scanEx

BLEのデバイスをスキャンして、指定したサービスを持つキャラクタリスティックを列挙します。

ESP1.0.2のBLEライブラリにはバグがあり、デバイスによってはハングアップしてしまうのと、同じCharacteristic UUIDを複数もつデバイスの場合、UUIDをキーにしたMapでしか受け取れないため黒魔術(#define private public)を使って無理やり拡張してあります。

### BLE_clientEx

BLEのデバイスをスキャンして、指定したサービスを持つキャラクタリスティックに通知を追加して、受信待ちをします。

ESP1.0.2のBLEライブラリにはバグがあり、デバイスによってはハングアップしてしまうのと、同じCharacteristic UUIDを複数もつデバイスの場合、UUIDをキーにしたMapでしか受け取れないため黒魔術(#define private public)を使って無理やり拡張してあります。
