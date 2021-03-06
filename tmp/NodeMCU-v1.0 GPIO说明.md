---
title: NodeMCU-v1.0 GPIO说明 
tags: 
grammar_cjkRuby: true
---
Author:Yang-YU
Date:2017-9-24

## 使用NodeMCU 的注意事项

在MicroPython和Lua脚本环境下，Pin口对应的地址是GPIO的标号

例如右上角的GPIO16口，连接着的LED在RST按键上方

``` Python 

import machine
from machine import Pin
 p16 = Pin(16,machine.Pin.OUT)
 p16.on()
 p16.off()
  ```
![](https://raw.githubusercontent.com/nodemcu/nodemcu-devkit/master/Documents/NODEMCU-DEVKIT-INSTRUCTION-EN.png)
IO index | ESP8266 pin    | IO index | ESP8266 pin|
----------- | -------------------- | ------------- | -------------------
D0			| GPIO16	|	D7 |  GPIO13
D1			| GPIO5		 |	 D8 |	GPIO15
D2			| GPIO4		 |	 D9 |	GPIO3
D3			| GPIO0		 |	 D10 |	GPIO1
D4			| GPIO2		 |	 D11 |	GPIO9
D5			| GPIO14	|	D12 |	GPIO10
D6			| GPIO12	| 	 
[管脚索引]
	
