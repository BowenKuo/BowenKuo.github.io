---
layout: post
title:  "在 Rstudio server 上加載 mxnet 時出現 Error.markdown"
date:   2017-10-13 13:30:00 +0800
categories: environment
tags: [lab, rstudio, mxnet]
---

將 mxnet 編譯安裝於 R 後, 在 Rstudio server include mxnet 出現以下錯誤
	
	> library(mxnet)
	Error: package or namespace load failed for ‘mxnet’:
	 .onLoad failed in loadNamespace() for 'mxnet', details:
	  call: dyn.load(file, DLLpath = DLLpath, ...)
	  error: unable to load shared object '/usr/lib64/R/library/mxnet/libs/libmxnet.so':
	  libcudart.so.8.0: cannot open shared object file: No such file or directory
	  
解決方法 : 在 command line 輸入 `sudo ldconfig /usr/local/cuda/lib64`


參考文件 : <https://github.com/tensorflow/tensorflow/issues/5343>
