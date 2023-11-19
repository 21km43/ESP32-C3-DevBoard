# ESP32-C3-DevBoard

ESP32-C3の開発ボード。USB CDC（内臓USBシリアル）を利用して書き込む。ESP32-C3のモジュールについてはESP32-C3-WROOM-02を使用している。モジュールは秋月電子などで購入可能。  
[秋月電子](https://akizukidenshi.com/catalog/g/gM-17493/)  
[DigiKey](https://www.digikey.jp/ja/products/detail/espressif-systems/ESP32-C3-WROOM-02-N4/14553031)

なお、基板発注、ESP32以外の部品実装に関しては、JLCPCBに発注することを想定している。ただし、ESP32-C3-WROOM-02に関してはStandard PCBAでしか実装してくれないので、Economic PCBAで発注するならばこの部品は実装しないように注意。

Espressif Libraryのインストールを前提としている（プラグイン＆コンテンツマネージャーからインストール可能）。

ガーバーファイル、BOM、CPLはpruductionフォルダに置いてある。

## 完成図
![image](/ESP32-C3-DevBoard.png)
