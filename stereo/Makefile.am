NULL =

sounddir = $(datadir)/sounds/freedesktop/stereo

sound_DATA =                            \
	audio-channel-front-center.ogg	\
	audio-channel-front-left.ogg	\
	audio-channel-front-right.ogg	\
	audio-channel-rear-center.ogg	\
	audio-channel-rear-left.ogg	\
	audio-channel-rear-right.ogg	\
	audio-channel-side-left.ogg	\
	audio-channel-side-right.ogg	\
	audio-test-signal.ogg		\
	audio-volume-change.ogg		\
	battery-full.ogg		\
	battery-low.ogg			\
	bell.ogg			\
	button-pressed.ogg		\
	button-toggle.ogg		\
	camera-shutter.ogg		\
	complete.ogg			\
	desktop-login.ogg		\
	desktop-logout.ogg		\
	desktop-switch-left.ogg		\
	desktop-switch-right.ogg 	\
	device-added.ogg		\
	device-removed.ogg		\
	dialog-cancel.ogg		\
	dialog-error.ogg		\
	dialog-information.ogg		\
	dialog-ok.ogg			\
	dialog-question.ogg		\
	dialog-warning.ogg		\
	link-pressed.ogg		\
	menu-click.ogg			\
	menu-popup.ogg			\
	message-new-email.ogg		\
	message-new-instant.ogg		\
	phone-incoming-call.ogg		\
	phone-outgoing-busy.ogg		\
	service-login.ogg		\
	service-logout.ogg		\
	suspend-error.ogg		\
	system-ready.ogg		\
	system-shutdown.ogg		\
	trash-empty.ogg			\
	window-attention.ogg		\
	window-close.ogg		\
	window-maximized.ogg		\
	window-minimized.ogg		\
	window-move-start.ogg		\
	window-move-stop.ogg		\
	window-slide.ogg		\
	window-unmaximized.ogg		\
	window-unminimized.ogg		\
	$(NULL)

install-data-hook:
	-rm -f $(DESTDIR)$(sounddir)/power-plug.ogg
	$(LN_S) device-added.ogg $(DESTDIR)$(sounddir)/power-plug.ogg
	-rm -f $(DESTDIR)$(sounddir)/power-unplug.ogg
	$(LN_S) device-removed.ogg $(DESTDIR)$(sounddir)/power-unplug.ogg
	-rm -f $(DESTDIR)$(sounddir)/network-connectivity-established.ogg
	$(LN_S) device-added.ogg $(DESTDIR)$(sounddir)/network-connectivity-established.ogg
	-rm -f $(DESTDIR)$(sounddir)/network-connectivity-lost.ogg
	$(LN_S) device-removed.ogg $(DESTDIR)$(sounddir)/network-connectivity-lost.ogg
	-rm -f $(DESTDIR)$(sounddir)/tooltip-popup.ogg
	$(LN_S) menu-popup.ogg $(DESTDIR)$(sounddir)/tooltip-popup.ogg
	-rm -f $(DESTDIR)$(sounddir)/screen-capture.ogg
	$(LN_S) camera-shutter.ogg $(DESTDIR)$(sounddir)/screen-capture.ogg

EXTRA_DIST =            \
	$(sound_DATA)	\
	$(NULL)

DISTCLEANFILES = \
	$(NULL)

MAINTAINERCLEANFILES =		\
	*~			\
	Makefile.in		\
	$(NULL)
