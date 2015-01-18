ACLOCAL_AMFLAGS = -I m4

lib_LIBRARIES = libSTM32F4_HAL.a

libSTM32F4_HAL_a_CFLAGS = \
    -fmessage-length=0 -fsigned-char -ffunction-sections -fdata-sections -fno-move-loop-invariants \
    -Wall -Wextra \
    -I$(top_srcdir)/include

HAL_INCLUDES = \
    core_cm4.h \
    core_cm4_simd.h \
    core_cmFunc.h \
    core_cmInstr.h \
    stm32f4xx_hal.h \
    stm32f4xx_hal_adc.h \
    stm32f4xx_hal_adc_ex.h \
    stm32f4xx_hal_can.h \
    stm32f4xx_hal_conf.h \
    stm32f4xx_hal_cortex.h \
    stm32f4xx_hal_crc.h \
    stm32f4xx_hal_cryp.h \
    stm32f4xx_hal_cryp_ex.h \
    stm32f4xx_hal_dac.h \
    stm32f4xx_hal_dac_ex.h \
    stm32f4xx_hal_dcmi.h \
    stm32f4xx_hal_def.h \
    stm32f4xx_hal_dma.h \
    stm32f4xx_hal_dma2d.h \
    stm32f4xx_hal_dma_ex.h \
    stm32f4xx_hal_eth.h \
    stm32f4xx_hal_flash.h \
    stm32f4xx_hal_flash_ex.h \
    stm32f4xx_hal_flash_ramfunc.h \
    stm32f4xx_hal_gpio.h \
    stm32f4xx_hal_gpio_ex.h \
    stm32f4xx_hal_hash.h \
    stm32f4xx_hal_hash_ex.h \
    stm32f4xx_hal_hcd.h \
    stm32f4xx_hal_i2c.h \
    stm32f4xx_hal_i2c_ex.h \
    stm32f4xx_hal_i2s.h \
    stm32f4xx_hal_i2s_ex.h \
    stm32f4xx_hal_irda.h \
    stm32f4xx_hal_iwdg.h \
    stm32f4xx_hal_ltdc.h \
    stm32f4xx_hal_nand.h \
    stm32f4xx_hal_nor.h \
    stm32f4xx_hal_pccard.h \
    stm32f4xx_hal_pcd.h \
    stm32f4xx_hal_pcd_ex.h \
    stm32f4xx_hal_pwr.h \
    stm32f4xx_hal_pwr_ex.h \
    stm32f4xx_hal_rcc.h \
    stm32f4xx_hal_rcc_ex.h \
    stm32f4xx_hal_rng.h \
    stm32f4xx_hal_rtc.h \
    stm32f4xx_hal_rtc_ex.h \
    stm32f4xx_hal_sai.h \
    stm32f4xx_hal_sd.h \
    stm32f4xx_hal_sdram.h \
    stm32f4xx_hal_smartcard.h \
    stm32f4xx_hal_spi.h \
    stm32f4xx_hal_sram.h \
    stm32f4xx_hal_tim.h \
    stm32f4xx_hal_tim_ex.h \
    stm32f4xx_hal_uart.h \
    stm32f4xx_hal_usart.h \
    stm32f4xx_hal_wwdg.h \
    stm32f4xx_ll_fmc.h \
    stm32f4xx_ll_fsmc.h \
    stm32f4xx_ll_sdmmc.h \
    stm32f4xx_ll_usb.h
    
libSTM32F4_HAL_a_SOURCES = \
    src/stm32f4xx_hal.c \
    src/stm32f4xx_hal_adc.c \
    src/stm32f4xx_hal_adc_ex.c \
    src/stm32f4xx_hal_can.c \
    src/stm32f4xx_hal_cortex.c \
    src/stm32f4xx_hal_crc.c \
    src/stm32f4xx_hal_cryp.c \
    src/stm32f4xx_hal_cryp_ex.c \
    src/stm32f4xx_hal_dac.c \
    src/stm32f4xx_hal_dac_ex.c \
    src/stm32f4xx_hal_dcmi.c \
    src/stm32f4xx_hal_dma.c \
    src/stm32f4xx_hal_dma2d.c \
    src/stm32f4xx_hal_dma_ex.c \
    src/stm32f4xx_hal_eth.c \
    src/stm32f4xx_hal_flash.c \
    src/stm32f4xx_hal_flash_ex.c \
    src/stm32f4xx_hal_flash_ramfunc.c \
    src/stm32f4xx_hal_gpio.c \
    src/stm32f4xx_hal_hash.c \
    src/stm32f4xx_hal_hash_ex.c \
    src/stm32f4xx_hal_hcd.c \
    src/stm32f4xx_hal_i2c.c \
    src/stm32f4xx_hal_i2c_ex.c \
    src/stm32f4xx_hal_i2s.c \
    src/stm32f4xx_hal_i2s_ex.c \
    src/stm32f4xx_hal_irda.c \
    src/stm32f4xx_hal_iwdg.c \
    src/stm32f4xx_hal_ltdc.c \
    src/stm32f4xx_hal_nand.c \
    src/stm32f4xx_hal_nor.c \
    src/stm32f4xx_hal_pccard.c \
    src/stm32f4xx_hal_pcd.c \
    src/stm32f4xx_hal_pcd_ex.c \
    src/stm32f4xx_hal_pwr.c \
    src/stm32f4xx_hal_pwr_ex.c \
    src/stm32f4xx_hal_rcc.c \
    src/stm32f4xx_hal_rcc_ex.c \
    src/stm32f4xx_hal_rng.c \
    src/stm32f4xx_hal_rtc.c \
    src/stm32f4xx_hal_rtc_ex.c \
    src/stm32f4xx_hal_sai.c \
    src/stm32f4xx_hal_sd.c \
    src/stm32f4xx_hal_sdram.c \
    src/stm32f4xx_hal_smartcard.c \
    src/stm32f4xx_hal_spi.c \
    src/stm32f4xx_hal_sram.c \
    src/stm32f4xx_hal_tim.c \
    src/stm32f4xx_hal_tim_ex.c \
    src/stm32f4xx_hal_uart.c \
    src/stm32f4xx_hal_usart.c \
    src/stm32f4xx_hal_wwdg.c \
    src/stm32f4xx_ll_fmc.c \
    src/stm32f4xx_ll_fsmc.c \
    src/stm32f4xx_ll_sdmmc.c \
    src/stm32f4xx_ll_usb.c

# Copy header files from "$srcdir/include" directory to "$DESTDIR/include/STM32F4"
# directory while preserving original directory tree structure.
install-data-local:
	@for f in $(HAL_INCLUDES); do \
	  d=`dirname $$f`; \
	  $(mkinstalldirs) $(DESTDIR)$(includedir)/STM32F4/$$d; \
	  p=$(srcdir)/include/$$f; \
	  $(INSTALL_DATA) $$p $(DESTDIR)$(includedir)/STM32F4/$$f; \
	done
