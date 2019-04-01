#
# Copyright (c) 2019 SUSE LLC. All Rights Reserved.
#

TOPDIR = ../..
include $(TOPDIR)/include/builddefs

CEPHFS_DIR = cephfs
TARGET_DIR = $(PKG_LIB_DIR)/$(TESTS_DIR)/$(CEPHFS_DIR)

include $(BUILDRULES)

install:
	$(INSTALL) -m 755 -d $(TARGET_DIR)
	$(INSTALL) -m 755 $(TESTS) $(TARGET_DIR)
	$(INSTALL) -m 644 group $(TARGET_DIR)
	$(INSTALL) -m 644 $(OUTFILES) $(TARGET_DIR)

# Nothing.
install-dev install-lib:
