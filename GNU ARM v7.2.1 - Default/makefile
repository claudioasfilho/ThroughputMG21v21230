################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include protocol/bluetooth/lib/EFR32MG21/GCC/subdir.mk
-include platform/emlib/src/subdir.mk
-include platform/emdrv/sleep/src/subdir.mk
-include platform/emdrv/nvm3/src/subdir.mk
-include platform/emdrv/gpiointerrupt/src/subdir.mk
-include platform/Device/SiliconLabs/EFR32MG21/Source/GCC/subdir.mk
-include platform/Device/SiliconLabs/EFR32MG21/Source/subdir.mk
-include lcd-graphics/subdir.mk
-include hardware/kit/common/drivers/subdir.mk
-include hardware/kit/common/bsp/subdir.mk
-include app/bluetooth/common/util/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: ThroughputMG21v21230.axf

# Tool invocations
ThroughputMG21v21230.axf: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: GNU ARM C Linker'
	arm-none-eabi-gcc -g -gdwarf-2 -mcpu=cortex-m33 -mthumb -T "/Users/clfilho/SimplicityStudio/NM_workspace/ThroughputMG21v21230/efr32mg21a010f1024im32.ld" -Xlinker --gc-sections -Xlinker -Map="ThroughputMG21v21230.map" -mfpu=fpv5-sp-d16 -mfloat-abi=hard --specs=nano.specs -o ThroughputMG21v21230.axf -Wl,--start-group "./app/bluetooth/common/util/infrastructure.o" "./app.o" "./app_master.o" "./app_slave.o" "./app_utils.o" "./application_properties.o" "./gatt_db.o" "./init_app.o" "./init_board.o" "./init_mcu.o" "./main.o" "./pti.o" "./hardware/kit/common/bsp/bsp_stk.o" "./hardware/kit/common/drivers/retargetio.o" "./hardware/kit/common/drivers/retargetserial.o" "./lcd-graphics/bmp.o" "./lcd-graphics/display.o" "./lcd-graphics/displayls013b7dh03.o" "./lcd-graphics/displaypalemlib.o" "./lcd-graphics/dmd_display.o" "./lcd-graphics/glib.o" "./lcd-graphics/glib_bitmap.o" "./lcd-graphics/glib_circle.o" "./lcd-graphics/glib_font_narrow_6x8.o" "./lcd-graphics/glib_font_normal_8x8.o" "./lcd-graphics/glib_font_number_16x20.o" "./lcd-graphics/glib_line.o" "./lcd-graphics/glib_polygon.o" "./lcd-graphics/glib_rectangle.o" "./lcd-graphics/glib_string.o" "./lcd-graphics/graphics.o" "./lcd-graphics/udelay.o" "./platform/Device/SiliconLabs/EFR32MG21/Source/GCC/startup_efr32mg21.o" "./platform/Device/SiliconLabs/EFR32MG21/Source/system_efr32mg21.o" "./platform/emdrv/gpiointerrupt/src/gpiointerrupt.o" "./platform/emdrv/nvm3/src/nvm3_default.o" "./platform/emdrv/nvm3/src/nvm3_hal_flash.o" "./platform/emdrv/nvm3/src/nvm3_lock.o" "./platform/emdrv/sleep/src/sleep.o" "./platform/emlib/src/em_assert.o" "./platform/emlib/src/em_burtc.o" "./platform/emlib/src/em_cmu.o" "./platform/emlib/src/em_core.o" "./platform/emlib/src/em_cryotimer.o" "./platform/emlib/src/em_crypto.o" "./platform/emlib/src/em_emu.o" "./platform/emlib/src/em_eusart.o" "./platform/emlib/src/em_gpio.o" "./platform/emlib/src/em_i2c.o" "./platform/emlib/src/em_msc.o" "./platform/emlib/src/em_rmu.o" "./platform/emlib/src/em_rtcc.o" "./platform/emlib/src/em_se.o" "./platform/emlib/src/em_system.o" "./platform/emlib/src/em_timer.o" "./platform/emlib/src/em_usart.o" "/Users/clfilho/SimplicityStudio/NM_workspace/ThroughputMG21v21230/protocol/bluetooth/lib/EFR32MG21/GCC/libmbedtls.a" "/Users/clfilho/SimplicityStudio/NM_workspace/ThroughputMG21v21230/platform/emdrv/nvm3/lib/libnvm3_CM33_gcc.a" "/Users/clfilho/SimplicityStudio/NM_workspace/ThroughputMG21v21230/protocol/bluetooth/lib/EFR32MG21/GCC/binapploader.o" "/Users/clfilho/SimplicityStudio/NM_workspace/ThroughputMG21v21230/platform/radio/rail_lib/autogen/librail_release/librail_efr32xg21_gcc_release.a" "/Users/clfilho/SimplicityStudio/NM_workspace/ThroughputMG21v21230/protocol/bluetooth/lib/EFR32MG21/GCC/libbluetooth.a" -lm -Wl,--end-group -Wl,--start-group -lgcc -lc -lnosys -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

	@echo 'Building hex file: ThroughputMG21v21230.hex'
	arm-none-eabi-objcopy -O ihex "ThroughputMG21v21230.axf" "ThroughputMG21v21230.hex"
	@echo ' '

	@echo 'Building bin file: ThroughputMG21v21230.bin'
	arm-none-eabi-objcopy -O binary "ThroughputMG21v21230.axf" "ThroughputMG21v21230.bin"
	@echo ' '

	@echo 'Building s37 file: ThroughputMG21v21230.s37'
	arm-none-eabi-objcopy -O srec "ThroughputMG21v21230.axf" "ThroughputMG21v21230.s37"
	@echo ' '

	@echo 'Running size tool'
	arm-none-eabi-size "ThroughputMG21v21230.axf"
	@echo ' '

# Other Targets
clean:
	-$(RM) $(EXECUTABLES)$(OBJS)$(C_DEPS) ThroughputMG21v21230.axf
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
