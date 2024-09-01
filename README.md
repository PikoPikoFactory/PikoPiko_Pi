# PikoPiko_Pi

![outlineiimage](/Image/PikoPiko_Pi.jpg)


## About this page
- Raspberry Pi ベアメタル MIDI シンセサイザー mt32-pi 専用HAT の情報ページです。
- 別途Raspberry Pi 3以降、もしくは、Raspberry Pi Zero 2以降が必要です。

## 回路図

[Schematics](/Hardware/mt32-pi-uHAT_schematic.pdf)

## 基板パターン図

[PCB Pattern](/Hardware/mt32-pi-uHAT_pattern.pdf)

## ソフトウェア

- https://github.com/dwhinham/mt32-pi より入手可能です。

## SDカードの作り方

- https://github.com/dwhinham/mt32-pi/releases より最新版のAssetsをダウンロードします。2024/9/1現在は　https://github.com/dwhinham/mt32-pi/releases/download/v0.13.1/mt32-pi-0.13.1.zip です。
- zipファイルを解凍して、中身を別途用意したmicro SDカードにコピーします。
- 設定ファイル mt32-pi.cfg に変更を加えます。以下の項目を書き換えます。
> usb = off
>  output_device = i2s  
> scheme = simple_buttons  
> type = ssd1306_i2c  
> height = 64  

- 変更した設定ファイルを以下に置きます。  
 [mt32-pi.cfg](/Software/mt32-pi.cfg)

## 接続
- MIDI INにMIDI機器のMIDI OUTを接続します。
- LINE OOUT（PCM5102A基板上)にアンプ等を接続します。ヘッドホンは直接駆動できません。
- MIDI OUTは何も接続しません。

## スイッチ操作
- VOLUME UP/DOWNの文字が入れ替わっています。修正方法は配線をカットして入れ替えるか、シルクの上にシールなどを貼るしかありません。申し訳ございません。
- ROMはMT-32 ROM と SoundFontの切り替えです。MT32 ROMは別途用意する必要があります。  
- FONTはSound Fontの切り替えです。Assetsには１種類しか入っていませんので、切り替えたい場合は別途用意する必要があります。

  
