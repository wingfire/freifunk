#
# Copyright (C) 2010 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=autofreifunk
PKG_VERSION:=1
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/autofreifunk
  SECTION:=freifunk
  CATEGORY:=Freifunk
  DEPENDS:=+luci +luci-ssl +batmand +freifunk-p2pblock +freifunk-firewall +openvpn
  TITLE:=freifunk installer
  PKGARCH:=all
endef

define Package/autofreifunk/description
  Installes all packages neccessary for freifunk
endef

define Build/Compile
endef

define Build/Configure
endef

define Package/autofreifunk/install
endef

$(eval $(call BuildPackage,autofreifunk))
