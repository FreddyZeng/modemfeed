include $(TOPDIR)/rules.mk

PKG_NAME:=xmm-modem
PKG_VERSION:=0.1.5
PKG_RELEASE:=1
PKG_MAINTAINER:=Konstantine Shevlakov <shevlakov@132lan.ru>

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  PKGARCH:=all
  DEPENDS:=+comgt +kmod-usb-acm +kmod-usb-serial-option \
	+kmod-usb-net-cdc-ncm +kmod-usb-net-rndis
  TITLE:=Fibocom L850/L860/FM350 protocol
endef

define Package/$(PKG_NAME)/description
	Simple connect to cellular for Fibocom L850/L860/FM350 module.
	Intel XMM LTE-A 7360/7560 and MediaTek T700 chipsets
endef


define Build/Prepare
endef

define Build/Configure
endef

define Build/Compile
endef


define Package/$(PKG_NAME)/install
	$(CP) ./root/* $(1)/
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
