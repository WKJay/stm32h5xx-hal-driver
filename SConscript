from building import *
import os

cwd = GetCurrentDir()
path = [os.path.join(cwd, 'Inc')]
src_path = os.path.join(cwd, 'Src')

CPPDEFINES = ['USE_HAL_DRIVER']

src = [
os.path.join(src_path, 'stm32h5xx_hal.c'),
os.path.join(src_path, 'stm32h5xx_hal_comp.c'),
os.path.join(src_path, 'stm32h5xx_hal_cortex.c'),
os.path.join(src_path, 'stm32h5xx_hal_crc.c'),
os.path.join(src_path, 'stm32h5xx_hal_crc_ex.c'),
os.path.join(src_path, 'stm32h5xx_hal_cryp.c'),
os.path.join(src_path, 'stm32h5xx_hal_cryp_ex.c'),
os.path.join(src_path, 'stm32h5xx_hal_dma.c'),
os.path.join(src_path, 'stm32h5xx_hal_dma_ex.c'),
os.path.join(src_path, 'stm32h5xx_hal_exti.c'),
os.path.join(src_path, 'stm32h5xx_hal_pwr.c'),
os.path.join(src_path, 'stm32h5xx_hal_pwr_ex.c'),
os.path.join(src_path, 'stm32h5xx_hal_rcc.c'),
os.path.join(src_path, 'stm32h5xx_hal_rcc_ex.c'),
os.path.join(src_path, 'stm32h5xx_hal_rng.c'),
os.path.join(src_path, 'stm32h5xx_hal_gpio.c'),
os.path.join(src_path, 'stm32h5xx_hal_icache.c'),
]

if GetDepend(['RT_USING_SERIAL']) or GetDepend(['RT_USING_NANO', 'RT_USING_CONSOLE']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_uart.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_uart_ex.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_usart.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_usart_ex.c')]
    

if GetDepend(['RT_USING_I2C']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_i2c.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_i2c_ex.c')]

if GetDepend(['RT_USING_SPI']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_spi.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_spi_ex.c')]

if GetDepend(['RT_USING_USB']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_hcd.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_pcd.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_pcd_ex.c')]
    src += [os.path.join(src_path, 'stm32h5xx_ll_usb.c')]

if GetDepend(['RT_USING_CAN']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_can.c')]

if GetDepend(['RT_USING_HWTIMER']) or GetDepend(['RT_USING_PWM']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_lptim.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_tim.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_tim_ex.c')]

if GetDepend(['RT_USING_ADC']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_adc.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_adc_ex.c')]
    
if GetDepend(['RT_USING_DAC']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_dac.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_dac_ex.c')]

if GetDepend(['RT_USING_RTC']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_rtc.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_rtc_ex.c')]

if GetDepend(['RT_USING_WDT']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_iwdg.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_wwdg.c')]

if GetDepend(['RT_USING_SDIO']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_sd.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_sd_ex.c')]
    src += [os.path.join(src_path, 'stm32h5xx_ll_sdmmc.c')]
    
if GetDepend(['RT_USING_AUDIO']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_sai.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_sai_ex.c')]
 
if GetDepend(['RT_USING_MTD_NOR']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_nor.c')]

if GetDepend(['RT_USING_MTD_NAND']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_nand.c')]

if GetDepend(['RT_USING_PM']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_lptim.c')]

if GetDepend(['BSP_USING_ON_CHIP_FLASH']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_flash.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_flash_ex.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_flash_ramfunc.c')]

if GetDepend(['BSP_USING_FMC']):
    src += [os.path.join(src_path, 'stm32h5xx_ll_fmc.c')]

if GetDepend(['BSP_USING_GFXMMU']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_gfxmmu.c')]

if GetDepend(['BSP_USING_DSI']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_dsi.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_dma2d.c')]
    src += [os.path.join(src_path, 'stm32h5xx_ll_dma2d.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_ltdc.c')]
    src += [os.path.join(src_path, 'stm32h5xx_hal_ltdc_ex.c')]

if GetDepend(['BSP_USING_SRAM']):
    src += [os.path.join(src_path, 'stm32h5xx_hal_sram.c')]
    src += [os.path.join(src_path, 'stm32h5xx_ll_fmc.c')]
    
group = DefineGroup('STM32H5-HAL', src, depend = ['PKG_USING_STM32H5_HAL_DRIVER'], CPPPATH = path, CPPDEFINES = CPPDEFINES)

Return('group')
