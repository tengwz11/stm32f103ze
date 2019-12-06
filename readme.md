##请先阅读[Mac下stm32开发(clion)](https://zhuanlan.zhihu.com/p/95498261)


1. 所有代码基于`正点原子-精英板` b站[教学视频链接](https://www.bilibili.com/video/av8938442?from=search&seid=6964447435862961564)
2. mcu型号:`STM32F103ZET6`, 各种配置基于开发板原理图进行配置


## 1.LED

> 实现点亮两个led灯

1. `LED0` 对应 `PB5` 口, `LED1` 对应 `PE5`口。 
2. 在STM32CubeMX中配置好两个IO口为输出,默认`高电平` led熄灭
3. 代码生成后, `main` 函数中将IO设置为低电平，点亮led