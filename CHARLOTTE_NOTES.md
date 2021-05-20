# charlotte's NetBSD notes

- needed to make a python3->python3.8 symlink
- requires math/py-numpy
- requires devel/py-cython
- requires graphics/py-Pillow
- needed to install graphics/freetype2 on purpose?? => needed to
  `USE_BUILTIN.freetype2=no` in mk.conf
- requires textproc/py-jinja2

#export CMAKE_MODULE_PATH=/usr/pkg/qt5/lib/cmake/Qt5Core:${CMAKE_MODULE_PATH}

export CMAKE_PREFIX_PATH=/usr/pkg/qt5
