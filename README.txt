README.txt

Description :

-- 使用WSL305S模块测试RSSI


Module : WSL305S
IDE : Keil_v5


Change Log:

-- 44211200 - WSL305S(Nov 2 2018 15:57:45):
	-- First Commit
    -- 程序由ST官方STM32L053R8-Nucleo移植而来, 主要修改如下:
        -- 修改 SPI, DIO, ANT_SWITCH GPIO接口 (Core/inc/stm32l0xx_hw_conf.h)
        -- 屏蔽所有关于 ADC 的模块 (Core/src/stm32l0xx_hw.c)
        -- 修改 Tx 功率为20dB, 修改 ANT_SWITCH 驱动以支持双IO口驱动 (Drivers/WSL305S/WSL305S.c)
        -- 修改 ChannelsDefaultMask (Middlewares/Third_Party/LoRaWAN/Mac/region/RegionCN470.c)
        -- 修改 CN470_MAX_NB_CHANNELS (Middlewares/Third_Party/LoRaWAN/Mac/region/RegionCN470.h)
        -- 删除原有 BSP 器件驱动(User/inc/bsp.h, User/src/bsp.c)
        -- 修改主控硬件宏定义 (User/inc/hw_conf.h)
        -- 删除多余 DEBUG 模式下多余的IO接口 (User/src/debug.c)


Author         : Jackie Yang
Email          : jackie.yang@liteon.com
Tel            : 86-0519-83068888 Ext 20013
Date           : 02/11/2018
