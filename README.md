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

-https://github.com/dwhinham/mt32-pi より入手可能です。

## SDカードの作り方

- https://github.com/dwhinham/mt32-pi/releases より最新版のAssetsをダウンロードします。2024/9/1現在は　https://github.com/dwhinham/mt32-pi/releases/download/v0.13.1/mt32-pi-0.13.1.zip です。
- zipファイルを解凍して、中身を別途用意したmicro SDカードにコピーします。
- 設定ファイル mt32-pi.cfg に変更を加えます。
-- usb = off
  output_device = i2s
  scheme = simple_buttons
  type = ssd1306_i2c
  height = 64

  ## SDカードの作り方
  
  
   
- 
