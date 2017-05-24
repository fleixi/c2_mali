libdir := ${D}/usr/lib/opengl/mali

install:
	# Mali Binaries
	rm -fr $(libdir)/libmali.so
	cp -aRP mali_libs/* $(libdir)/lib
	touch $(libdir)/.gles-only
