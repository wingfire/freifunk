#
# Copyright (C) 2010 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ff-koeln-bonn
PKG_VERSION:=1
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/ff-koeln-bonn
  SECTION:=freifunk
  CATEGORY:=Freifunk
  DEPENDS:=+autofreifunk
  TITLE:=configurations for freifunk koeln / bonn
  PKGARCH:=all
endef

define Package/ff-koeln-bonn/description
  Installes all configuration needed for freifunk koeln / bonn
endef

define Build/Compile
endef

define Build/Configure
endef

define Package/ff-koeln-bonn/install
	$(INSTALL_DIR) $(1)/etc/openvpn
	$(INSTALL_DATA) ./files/openvpn/ca.crt $(1)/etc/openvpn
        $(INSTALL_DATA) ./files/openvpn/client.conf $(1)/etc/openvpn
        $(INSTALL_DATA) ./files/openvpn/contest $(1)/etc/openvpn
        $(INSTALL_DATA) ./files/openvpn/freifunkknoten.crt $(1)/etc/openvpn
        $(INSTALL_DATA) ./files/openvpn/freifunkknoten.key $(1)/etc/openvpn
	$(INSTALL_DATA) ./files/luci $(1)/etc/config/openvpn
endef

$(eval $(call BuildPackage,ff-koeln-bonn))
