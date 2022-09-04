# 基于stm32的指纹锁识别系统  
  该项目采用了stm32和海凌科的HLK-ZW651半导体指纹模块
  
### 指纹模块简介
　　HLK-ZW651半导体指纹模块是集成了半导体传感器和指纹算法芯片为一体化指纹处理模块，具有体积小、功耗低、接口简单等特点，模块可靠性高、干湿手指适应性好，指纹搜索速度快。  
　　指纹图像读取时，对干湿手指都有灵敏的反应和判断，能获得最佳的成像质量，适用人群广泛。 具备自学习功能，实际使用过程中越用越好用。  
　　HLK-ZW651 模块还具备感应手指功能，当手指按压到指纹采集面时，模块 Touch 脚输出高电平。 HLK-ZW651 模块通讯接口为 UART 接口, 本模块作为从设备，由主设备发送相关命令对其进行控制。该模块具有可调节的安全等级功能、指纹特征数据的读/写功能。  
  指纹模块实物图：
![正面](https://github.com/willow017/fingerprint_lock/blob/main/1.png) ![反面](https://github.com/willow017/fingerprint_lock/blob/main/0.png)  
### 主要功能  
　　主要实现了指纹注册、指纹验证、查看指纹个数、删除指纹、清除所有指纹
### 技术栈  
　　stm32、usart、中断
### stm32f103rc与海凌科HLK-ZW651指纹模块连线表
　引脚名     　　          stm32F103RC芯片IO口  
VCC3_3V           　　 　　          3V3  
INT_OUT            　　    　　        PB1  
MCU3_3V              　　      　　    3V3  
TTL_TXD               　　         　　PA3  
TTL_RXD                　　       　　 PA2  
　GND                  　　         　 GND  
