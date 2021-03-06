---
ID: 28
post_title: Download
author: David Coeurjolly
post_date: 2010-10-13 12:44:48
post_excerpt: ""
layout: page
permalink: http://dgtal.org/download/
published: true
gr_overridden:
  - "0"
---
### Releases

*   Last stable DGtal release: [DGtal-0.9.0-Source.tar.gz][1]
*   [All releases][2]

### Development version

*   Read-only git access (development branch): ```git clone git://github.com/DGtal-team/DGtal.git```
*   You can also browse the [source.][3]
*   If you want to contribute, please contact us or submit a proposal through a Github Pull-Request.

### Requirements

*   C++ compiler with C++11 features (gcc>=4.7, clang >= 3.0, VS14,...) 
*   [cmake][4] to generate the project and compile the library (>=2.6)
*   [boost][5] (>= 1.46)</ul> 
    
### Optional dependencies

*   [Gnu Multiprecision Arithmetic Library][6] (GMP) (arbitrarily large integers)
*   [libQGLViewer][7] interactive viewer of 3D objects (see "stream 3D" in the documentation), libQGLViewer would require to have OpenGL and QT4 installed on your system.
*   [CGAL][8] (to be able to consider point cloud based differential estimators).
*   [InsightToolkit][9] (ITK) to merge ITK pipelines in DGtal via the image container.
*   [GraphicsMagick ][10](to be able to load various image file formats)
*   [doxygen][11] (to generate the source code documentation)
*   C++ compiler with cpp0x instructions (gcc >= 4.4, Visual C++ 2010, ...)
    
### How to build the library
See also [ the dedicated page][12] in the DGtal documentation. 

*   Linux (command line) 
  *   get the code -> DGtal/
  *   ```mkdir build ; cd build ; cmake .. ; make```
  *   if you wish, you can "install" the library in your system: ```sudo make install```
*   Windows 
  *   use cmake-gui to generate the VS project for instance
  *   open the DGtal project and compile with Visual Studio (VS14 or above)

 [1]: http://dgtal.org/releases/DGtal-0.9-Source.tar.gz
 [2]: https://github.com/DGtal-team/DGtal/releases
 [3]: https://github.com/DGtal-team/DGtal
 [4]: http://www.cmake.org
 [5]: http://www.boost.org
 [6]: http://gmplib.org/
 [7]: http://www.libqglviewer.com/
 [8]: http://cgal.org/
 [9]: http://www.itk.org/
 [10]: http://www.graphicsmagick.org/
 [11]: http://www.stack.nl/~dimitri/doxygen/
 [12]: http://dgtal.org/doc/stable/moduleBuildDGtal.html
