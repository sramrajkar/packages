include $(TOPDIR)/rules.mk

PKG_NAME:=python-pymodbus
PKG_VERSION:=3.6.6
PKG_RELEASE:=1

PYPI_NAME:=pymodbus
PKG_HASH:=c4d556a0954d00a9e1c8f1d0de03f41c4800336e6d785e820f2917eeb4ee7736

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_DEPENDS:=python-setuptools-scm/host  # setuptools_scm[toml] >= 3.4.1

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-pymodbus
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Python Modbus
  URL:=https://pymodbus.readthedocs.io/en/latest/
  DEPENDS:=+python3-light
endef

define Package/python3-pymodbus/description
  A fully featured Modbus protocol stack in Python.
endef

$(eval $(call Py3Package,python3-pymodbus))
$(eval $(call BuildPackage,python3-pymodbus))
$(eval $(call BuildPackage,python3-pymodbus-src))