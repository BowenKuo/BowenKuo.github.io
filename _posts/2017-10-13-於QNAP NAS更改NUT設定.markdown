---
layout: post
title:  "2017-10-13-於QNAP\ NAS更改NUT設定.markdown
date:   2017-10-13 12:01:00 +0800
categories: environment
tags: [lab, nut, nas, qnap]
---

由於 Lab 使用的是 **QNAP TS-853A**, 內建 NUT (network USP tools) 只能與一台 UPS 連線, 但是 Lab 有兩台 UPS, 所以必須 ssh 進入 NAS 內更改 NUT 設定

NUT 設定放在 `/mnt/HDA_ROOT/.config/ups` 底下

	[~] # ls /mnt/HDA_ROOT/.config/ups
	ups.conf     upsd.conf    upsd.users   upsmon.conf
	

參考文件 : <https://forum.qnap.com/viewtopic.php?f=151&t=47493&sid=62f148925ede80f1a6e75c2a2ea328c7>
