AM_CPPFLAGS = -I$(top_srcdir)

noinst_HEADERS = \
	utils.hpp \
	server-conf.hpp

sbin_PROGRAMS = phosphor-rsyslog-conf

phosphor_rsyslog_conf_SOURCES = \
	main.cpp \
	server-conf.cpp

phosphor_rsyslog_conf_LDADD = \
	$(top_builddir)/sdjournal.o

phosphor_rsyslog_conf_LDFLAGS = \
	$(SDBUSPLUS_LIBS) \
	$(PHOSPHOR_DBUS_INTERFACES_LIBS) \
	-lstdc++fs

phosphor_rsyslog_conf_CXXFLAGS = \
	$(SDBUSPLUS_CFLAGS) \
	$(PHOSPHOR_DBUS_INTERFACES_CFLAGS) \
	-flto
