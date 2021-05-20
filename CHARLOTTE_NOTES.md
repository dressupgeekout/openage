# charlotte's NetBSD notes

- needed to make a python3->python3.8 symlink
- requires math/py-numpy
- requires devel/py-cython
- requires graphics/py-Pillow
- needed to install graphics/freetype2 on purpose?? => needed to
  `USE_BUILTIN.freetype2=no` in mk.conf in order to get py-Pillow to succeed
  (pkgsrc 2021Q1)
- requires textproc/py-jinja3

#export CMAKE_MODULE_PATH=/usr/pkg/qt5/lib/cmake/Qt5Core:${CMAKE_MODULE_PATH}

export CMAKE_PREFIX_PATH=/usr/pkg/qt5

- requires nyan, for real
- + devel/py-readline



		[  9%] Building CXX object libopenage/CMakeFiles/libopenage.dir/console/tests.cpp.o
		In file included from /home/charlotte/devel/openage/libopenage/console/tests.cpp:12:0:
		/home/charlotte/devel/openage/libopenage/console/../util/pty.h:15:12: fatal error: pty.h: No such file or directory
		 #  include <pty.h>
								^~~~~~~
		compilation terminated.
		*** Error code 1

		Stop.
		make[2]: stopped in /home/charlotte/devel/openage/build
		*** Error code 1

		Stop.
		make[1]: stopped in /home/charlotte/devel/openage/build
		*** Error code 1

		Stop.
		make: stopped in /home/charlotte/devel/openage/build

i bet you pty.h is a linux thing...

- i guess we also need libinotify -- otherwise, -DWANT_INOTIFY:BOOL=OFF
