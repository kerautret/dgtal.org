---
ID: 650
post_title: 'DGtal &#8211; Digital Geometry Tools and Algorithms'
author: David Coeurjolly
post_date: 2010-06-03 13:17:01
post_excerpt: ""
layout: page
permalink: http://dgtal.org/
published: true
gr_overridden:
  - "0"
ninja_forms_form:
  - "0"
---
### Project DGtal

The collaborative project [DGtal][3] aims at developing generic, efficient and reliable digital geometry data structures, algorithms and tools. It takes the form of an open-source C++ library DGtal and a set of tools and binaries DGtalTools.

### Overview of digital geometry

<a title="Digital Geometry" href="http://en.wikipedia.org/wiki/Digital_geometry">Digital geometry</a> aims at defining proper geometric models and properties onto subsets of the integer plane/space ($\mathbb{Z}^d$). It is also interested in defining efficient algorithms for digital object topology and geometry processing. Natural applications of digital geometry are found in <strong>image</strong> <strong>analysis</strong>, since images are digital by nature. Digital geometry finds also applications in pattern recognition, computer graphics, biomedical  image analysis, OCR, 3D imaging.


Even if the domain emerged during the second half of the 20th century with the birth of computer graphics and digital image processing, many links have been demonstrated between Digital Geometry results and fundamental theorems in mathematics (arithmetic, geometry, topology...), discrete mathematics (word theory, combinatorics, graph theory...) or computer science (algorithmic, computational geometry, image processing...).

Have a look to the <a title="Gallery" href="http://dgtal.org/gallery/">Gallery</a> for digital geometry illustrations in DGtal.

###  Objectives of DGtal Project

[DGtal][3] gathers in a unified setting many data structures and algorithms of digital geometry and related fields (digital topology, image processing, discrete geometry, arithmetic). It aims at fulfilling several objectives.

* It structures, in a unified and ready-to-use setting, different developments of the digital geometry and topology community.
* It makes easier the appropriation of our tools for neophytes (new PhD students, researchers from other fields, ...).
* It allows fair comparisons of new methods with already existing approaches.
* It constructs a federative project that stimulates research in this field.
* It facilitates the dissemination of digital geometry in other academic fields or in industrial applications.
* It simplifies the construction of demonstration tools, so as to share new results or demonstrate the potential efficiency of new algorithms.

### Packaging

The project is composed of two main packages: [DGtal ][1](main library) and [DGtalTools][2] which contains several tools built on DGtal. 

### Features Digital Geometry Tools and Algorithms 


[DGtal][3] offers concepts, data structures, algorithms for the following tasks: [digital spaces and sets][4] (integer plane and subsets, cellular grid space and subsets); [integers and fractions][5] (irreducible and continued fractions, Stern-Brocot tree); [digital straightness][6] (patterns, digital straight lines and subsegments); [grid curve representation][7] (points, pixel, interpixel, Freeman chaincode) and [analysis][8] (segmentation, covering); [primitives][9] (arithmetic, geometric and combinatorial digital straight segments, digital circular arc, digital planes);[ Euclidean and digital multigrid shape generation][10] (parametric and implicit curves and surfaces, Gauss digitization); [volumetric analysis with distance transformation][11] (DT and reverse DT, medial axis, digital Voronoi diagram); [geometric estimators][12] (tangent and curvature estimators along digital curves and surfaces); [digital topology][13] (adjacencies, objects, borders, simpleness, homotopic thinning); [digital surfaces][14] (implicit and explicit containers, neighborhood, tracking, dual surfaces, marching-cubes); [multi-variate polynomials][15]; [nD image processing][16] (readers, writers, vector, map and tree containers, ITK bridge); [export and visualization][17] (2D and 3D export and display stream mechanism; 3D interaction mechanism).

 [1]: http://dgtal.org/download/ "Download"
 [2]: http://dgtal.org/tools/ "Tools"
 [3]: http://dgtal.org "DGtal"
 [4]: http://dgtal.org/doc/nightly/packageKernel.html "digital spaces and sets"
 [5]: http://dgtal.org/doc/nightly/moduleIrreducibleFraction.html "integers and fractions"
 [6]: http://dgtal.org/doc/nightly/moduleDigitalStraightness.html "digital straightness"
 [7]: http://dgtal.org/doc/nightly/moduleGridCurveAnalysis.html "grid curve representation"
 [8]: http://dgtal.org/doc/nightly/moduleGridCurveAnalysis.html "analysis"
 [9]: http://dgtal.org/doc/nightly/packageGeometry.html "primitives"
 [10]: http://dgtal.org/doc/nightly/moduleShape.html " Euclidean and digital multigrid shape generation"
 [11]: http://dgtal.org/doc/nightly/moduleVolumetric.html "volumetric analysis with distance transformation"
 [12]: http://dgtal.org/doc/nightly/packageGeometry.html "geometric estimators"
 [13]: http://dgtal.org/doc/nightly/moduleDigitalTopology.html "digital topology"
 [14]: http://dgtal.org/doc/nightly/moduleDigitalSurfaces.html "digital surfaces"
 [15]: http://dgtal.org/doc/nightly/modulePolynomial.html "multi-variate polynomials"
 [16]: http://dgtal.org/doc/nightly/packageImage.html "nD image processing"
 [17]: http://dgtal.org/doc/nightly/packageIO.html "export and visualization"
