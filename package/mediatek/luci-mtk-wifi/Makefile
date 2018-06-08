include $(TOPDIR)/rules.mk

PKG_NAME:=luci-mtk-wifi
PKG_VERSION:=20180607
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/luci-mtk-wifi
  SECTION:=MTK Properties
  CATEGORY:=MTK Properties
  TITLE:=LuCI for MTK Wi-Fi drivers
  SUBMENU:=Applications
  DEPENDS:=+luci
endef

define Package/luci-mtk-wifi/description
  LuCI for MTK Wi-Fi drivers
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Compile/Default

endef
Build/Compile = $(Build/Compile/Default)

define Package/luci-mtk-wifi/install
	$(CP) -a files/* $(1)/
endef

$(eval $(call BuildPackage,luci-mtk-wifi))

