libdir := ${D}/usr/lib/opengl/mali
includedir := ${D}/usr/include
pkgconfigdir := $(libdir)/pkgconfig

install:
	# Mali Binaries
	rm -fr $(libdir)/libmali.so
	cp -aRP mali_libs/* $(libdir)
	
	# Mali Headers
	rm -rf $(includedir)/EGL $(includedir)/GLES $(includedir)/GLES2 $(includedir)/GLES3 $(includedir)/KHR
	cp -aRP mali_headers/* ${D}/usr/include
	
	# PKG Config
	rm -fr $(pkgconfigdir)/glesv*.pc $(pkgconfigdir)/egl.pc $(pkgconfigdir)/wayland-egl.pc $(pkgconfigdir)/OpenCL.pc $(pkgconfigdir)/gbm.pc
	cp -aRP ../pkgconfig/* $(pkgconfigdir)
	

		
