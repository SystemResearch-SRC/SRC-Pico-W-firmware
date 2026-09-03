# SRC-Pico-W-firmware
Firmware for Raspberry Pi Pico W that functions as a temperature monitor logger, collaborating with our official iOS app via BLE. 日本語：BLE通信で当社のiOSアプリと連携し、温度監視ロガーとして機能するRaspberry Pi Pico W用ファームウェア。

# Pico W Temperature Monitor Logger Firmware
Raspberry Pi Pico W を使用して周囲の温度を測定し、BLE（Bluetooth Low Energy）経由で自社のiOSアプリにデータを送信・記録するファームウェアです。

## 主な機能 (Features)
* **温度計測**: Pico Wの RP2040 内臓温度センサーを利用した温度監視
* **BLE通信**: iOSアプリへのリアルタイムデータ転送と過去ログの同期
* **スタンドアロン動作**: 市販の Pico W に書き込むだけで即座にロガーとして動作します

### 動作デモ・解説動画
https://www.youtube.com/watch?v=pLldfUf_v9I

## 連携iOSアプリ (Companion iOS App)
本ファームウェアは、App Storeで配信中の当社公式アプリと連携して動作します。
* **アプリ名**: BLE_TempLogger
* **App Storeリンク**: 

## 準備するもの (Prerequisites)
1. **Raspberry Pi Pico W** 本体 (市販品)
2. **Micro USB ケーブル** (データ通信対応のもの)
3. **PC環境**: Windows11など、Pico Wと接続して、ファームウェアの書き込みができるパソコン

## 導入手順 (Getting Started)
### 1. ファームウェアの書き込み
1. Pico Wに最新のファームウェア（src_templogger.uf2ファイル）を書き込みます。

### 2. iOSアプリとのペアリング
1. Pico W に電源を供給すると、自動的にBLEのペアリングモード（アドバタイズ）が開始されます。
2. iOS端末の Bluetooth を ON にします。
3. 公式iOSアプリを起動し、Home画面から Start Scan をクリックして、表示される Pico W を選択して接続してください。
