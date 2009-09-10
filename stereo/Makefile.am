NULL =

sounddir = $(datadir)/sounds/freedesktop/stereo

sound_DATA =                            \
	alarm-clock-elapsed.oga	        \
	audio-channel-front-center.oga	\
	audio-channel-front-left.oga	\
	audio-channel-front-right.oga	\
	audio-channel-rear-center.oga	\
	audio-channel-rear-left.oga	\
	audio-channel-rear-right.oga	\
	audio-channel-side-left.oga	\
	audio-channel-side-right.oga	\
	audio-test-signal.oga		\
	audio-volume-change.oga		\
	battery-full.oga		\
	battery-low.oga			\
	bell.oga			\
	button-pressed.oga		\
	button-toggle.oga		\
	camera-shutter.oga		\
	complete.oga			\
	desktop-login.oga		\
	desktop-logout.oga		\
	device-added.oga		\
	device-removed.oga		\
	dialog-cancel.oga		\
	dialog-error.oga		\
	dialog-information.oga		\
	dialog-ok.oga			\
	dialog-question.oga		\
	dialog-warning.oga		\
	link-pressed.oga		\
	message.oga			\
	message-new-instant.oga		\
	phone-incoming-call.oga		\
	phone-outgoing-busy.oga		\
	phone-outgoing-calling.oga      \
	service-login.oga		\
	service-logout.oga		\
	suspend-error.oga		\
	trash-empty.oga			\
	window-attention.oga		\
	window-new.oga                  \
	$(NULL)

install-data-hook:
	-rm -f $(DESTDIR)$(sounddir)/power-plug.oga
	$(LN_S) device-added.oga $(DESTDIR)$(sounddir)/power-plug.oga
	-rm -f $(DESTDIR)$(sounddir)/power-unplug.oga
	$(LN_S) device-removed.oga $(DESTDIR)$(sounddir)/power-unplug.oga
	-rm -f $(DESTDIR)$(sounddir)/network-connectivity-established.oga
	$(LN_S) device-added.oga $(DESTDIR)$(sounddir)/network-connectivity-established.oga
	-rm -f $(DESTDIR)$(sounddir)/network-connectivity-lost.oga
	$(LN_S) device-removed.oga $(DESTDIR)$(sounddir)/network-connectivity-lost.oga
	-rm -f $(DESTDIR)$(sounddir)/screen-capture.oga
	$(LN_S) camera-shutter.oga $(DESTDIR)$(sounddir)/screen-capture.oga

EXTRA_DIST =            \
	$(sound_DATA)	\
	$(NULL)

DISTCLEANFILES = \
	$(NULL)

MAINTAINERCLEANFILES =		\
	*~			\
	Makefile.in		\
	$(NULL)
