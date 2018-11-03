pySlipQt
========

pySlipQt is a 'slip map' widget for PyQt5.  You can use it to embed a tiled map
into your PyQt5 application.  The map can be overlayed with points, images, text
and other layers.  The map tiles can come from a local source of pre-generated
tiles or from a tile server.  The tiles may have any desired coordinate system
as tile coordinates are translated to pySlipQt internal coordinates.

pySlipQt works on Linux, Mac and Windows.  Requirements are python 3 and PyQt5.

For more information visit the
`GitHub repository <https://github.com/rzzzwilson/pySlipQt/>`_ or view the API
documentation in
`the wiki <https://github.com/rzzzwilson/pySlipQt/wiki/The-pySlipQt-API>`_.

Release Notes
-------------

Release 0.1 of pySlipQt is early-release and is therefore ALPHA software.  It
is being released at this early stage so anyone interested in pySlipQt can run
the "pyslipqt_demo.py" program and get comfortable with the way pySlipQt works.

This release has these warnings:

1. Little testing has been done, so please report any errors to me at 
   rzzzwilson@gmail.com and attach the "pyslipqt.log" file.

2. "Box selection" (a multi-selection made by dragging a select box) doesn't
   work at the moment, but it will!

3. Wrap-around of tiles doesn't work yet, but I *hope* to have it working even
   though it will come with some limitations.

4. The included GMT tileset is very old and has a different zoom compared to any
   tiles from the 'net, such as OSM tiles, for instance.  I hope to fix this
   later.  The GMT tiles can still be used an example of how to use locally
   generated tiles.

5. Many of the "examples/test_*.py" programs have not been converted to python3
   and PyQt5.  The programs that *do* work are:
       test_assumptions.py
       test_gmt_local_tiles.py
       test_osm_tiles.py
       test_display_text.py
       test_layer_control.py
       

The GMT example tileset is included in the "examples" subdirectory.  The
gmt_local_tiles.py tileset code assumes that the zip file has been unzipped in
the user's home directory (ie, ~/gmt_local_tiles).  If you put the tiles in any
other place, please make the appropriate changes in gmt_local_tiles.py or make
your own version of gmt_local_tiles.py.

See the API documentation for the details on how to use pySlipQt.  The
demonstration program "examples/pyslipqt_demo.py" does require that the pySlipQt
package has been installed, though you make run pyslipqt_demo.py from any place
as long as it is moved along with its required files from the "examples"
directory.