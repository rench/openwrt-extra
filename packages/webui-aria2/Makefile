#
# Copyright (C) 2014 shangjiyu <shangjiyu@gmail.com>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=webui-aria2
PKG_VERSION:=20151031
PKG_RELEASE:=2
PKG_MAINTAINER:=shangjiyu <shangjiyu@gmail.com>

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/kuoruan/webui-aria2.git
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)
PKG_SOURCE_VERSION:=c087af8e78f33903c2533c773010b0210509efcc
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION)-$(PKG_SOURCE_VERSION).tar.gz

include $(INCLUDE_DIR)/package.mk

define Package/webui-aria2
  SECTION:=net
  CATEGORY:=Network
  SUBMENU:=Download Manager
  DEPENDS:=+aria2
  TITLE:=An interface to interact with aria2
  URL:=https://github.com/ziahamza/webui-aria2
  PKGARCH:=all
endef

define Package/webui-aria2/description
	The aim for this project is to create the worlds best and hottest interface to interact with aria2. Very simple to use.
endef

define Build/Compile
endef

define Package/webui-aria2/install
	$(INSTALL_DIR) $(1)/www/webui-aria2
	$(CP) $(PKG_BUILD_DIR)/fonts $(1)/www/webui-aria2
	$(CP) $(PKG_BUILD_DIR)/js $(1)/www/webui-aria2
	$(CP) $(PKG_BUILD_DIR)/img $(1)/www/webui-aria2
	$(CP) $(PKG_BUILD_DIR)/css $(1)/www/webui-aria2
	$(CP) $(PKG_BUILD_DIR)/index.html $(1)/www/webui-aria2
	$(CP) $(PKG_BUILD_DIR)/favicon.ico $(1)/www/webui-aria2
endef

$(eval $(call BuildPackage,webui-aria2))
