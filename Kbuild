ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY), y)
dtbo-$(CONFIG_ARCH_WAIPIO)		+= waipio-camera.dtbo
#dtbo-$(CONFIG_ARCH_WAIPIO)		+= waipio-camera-overlay-v2.dtbo
#dtbo-$(CONFIG_ARCH_WAIPIO)		+= waipio-camera-sensor-mtp.dtbo \
#										waipio-camera-sensor-cdp.dtbo \
#										waipio-camera-sensor-qrd.dtbo

#PLUS_DTS_OVERLAY start
dtbo-$(CONFIG_ARCH_DIWALI)		+= diwali-camera.dtbo
dtbo-$(CONFIG_ARCH_DIWALI) += oplus/wuyi-21125-camera-diwali-overlay.dtbo

dtbo-$(CONFIG_ARCH_CAPE) += cape-camera.dtbo
dtbo-$(CONFIG_ARCH_CAPE) += oplus/udon_22803-camera-cape-overlay.dtbo
#OPLUS_DTS_OVERLAY end

else
$(error CONFIG_BUILD_ARM64_DT_OVERLAY is: $(CONFIG_BUILD_ARM64_DT_OVERLAY))
endif

always-y	:= $(dtbo-y) $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files	:= *.dtb *.dtbo
