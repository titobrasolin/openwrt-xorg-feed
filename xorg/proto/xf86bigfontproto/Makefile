#
# Copyright (C) 2006-2010 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
# blogic@openwrt.org

include $(TOPDIR)/rules.mk

PKG_NAME:=xf86bigfontproto
PKG_VERSION:=1.2.0
PKG_RELEASE:=3

PKG_SOURCE_URL:=http://xorg.freedesktop.org/releases/individual/proto/
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.bz2
PKG_BUILD_DIR:=$(BUILD_DIR)/Xorg/$(PKG_NAME)-$(PKG_VERSION)/
PKG_MD5SUM:=120e226ede5a4687b25dd357cc9b8efe

include $(INCLUDE_DIR)/package.mk

define Package/xf86bigfontproto
  SECTION:=xorg-proto
  CATEGORY:=Xorg
  SUBMENU:=proto
  DEPENDS:=
  TITLE:=xf86bigfontproto
  URL:=http://xorg.freedesktop.org/
endef

define Build/InstallDev
	DESTDIR="$(1)" $(MAKE) -C $(PKG_BUILD_DIR)/ $(MAKE_FLAGS) install
endef

define Build/Compile
	true
endef

$(eval $(call BuildPackage,xf86bigfontproto))
