include $(TOPDIR)/rules.mk

include ./uclibc.mk

source: uclibc-source
prepare: uclibc-configured
compile: $(UCLIBC_DIR)/lib/libc.a
install: uclibc
	rm -rf $(TARGET_DIR)/lib/libpthread*.so*
	$(STRIP) $(TARGET_DIR)/lib/*.so
clean: uclibc-toolclean
