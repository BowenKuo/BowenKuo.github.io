---
layout: post
title:  "在Github上利用Jekyll架設部落格"
date:   2017-10-12 02:15:49 +0800
categories: jekyll update
---

由於 Lab 使用的是 **QNAP TS-853A**, 內建 NUT (network USP tools) 只能與一台 UPS 連線, 但是 Lab 有兩台 UPS, 所以必須 ssh 進入 NAS 內更改 NUT 設定

NUT 設定放在 `/mnt/HDA_ROOT/.config/ups` 底下

	[~] # ls /mnt/HDA_ROOT/.config/ups
	ups.conf     upsd.conf    upsd.users   upsmon.conf
	

參考文件 : <https://forum.qnap.com/viewtopic.php?f=151&t=47493&sid=62f148925ede80f1a6e75c2a2ea328c7>
