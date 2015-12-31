---
ID: 394
post_title: DGtalTools
author:
  - David Coeurjolly
post_date:
  - 2012-06-04 19:15:26
post_excerpt:
  - ""
layout: page
permalink:
  - /tools/
published: true
w:
  - 'a:1:{i:0;s:1:"0";}'
gr_options:
  - 'a:1:{i:0;s:131:"a:3:{s:13:"enable-ribbon";s:4:"Show";s:10:"github-url";s:40:"https://github.com/DGtal-team/DGtalTools";s:11:"ribbon-type";s:1:"0";}";}'
---

[DGtalTools][1] is a separate github project containing tools constructed using DGtal library. The main goal of this part is to gather simple and useful tools exploiting the structures and algorithms defined in DGtal. The resulting tools could be useful to: 

* Share and apply DGtal algorithms to various data from different domains. 
* Construct demonstration tools like online demonstrations (as for instance the one of the [Image Processing Online][2]). 
* Simplify comparisons of different algorithms with an single framework. 
* Provide useful tools of digital image related algorithms (extraction of connected components, digital contour/surface extraction, simple visualization tools...). 
 
The source code of the tools can also be used to non DGtal familiar user to show how to include the DGtal library framework directly in their own source code (in complement of

[ DGtal tutorial][3] ). At the moment the DGTal project is organized as follows (<span style="color: #8b0000">new</span> or <span style="color: #008b00">improved </span> from 0.9): 

* **converters/**: utilities to convert various simple file formats: 
 * <span style="color: #00008b">convertVol</span>: a simple generic volume image converters (can process actually pgm3d, vol, longvol, raw (for writing)). 
 * <span style="color: #00008b"> dicom2vol</span>: convert dicom images into 3d volumic file (need itk option in DGtal). 
 * <span style="color: #00008b"><span style="color: #008b00">freeman2img</span> </span>: transform one or several freeman chains into a pgm file by filling their interior areas. 
 * <span style="color: #00008b">freeman2sdp</span>: convert freeman chain towards a Sequence of Discrete Points. 
 * <span style="color: #00008b"> HDF52vol</span>: convert HDF5 to vol file format. 
 * <span style="color: #8b0000">heightfield2shading</span>: a new tool to render a 2D heightfield image into a shading one. 
 * <span style="color: #8b0000">heightfield2vol</span>: a new tool to transform 2D heightmap into volumetric file. 
 * <span style="color: #00008b">img2freeman</span>: to extract a freeman chain contour from a grayscale image. 
 * <span style="color: #8b0000">imgAddNoise</span>: a new tool to add noise (Kanungo's) to a binary 2D object. 
 * <span style="color: #8b0000">itk2vol</span>: convert any image of itk format (mhd, mha, ...) to vol (available with the itk option in DGtal).
 * <span style="color: #00008b"> longvol2vol</span>: convert longvol to vol file using different conversion policies. 
 * <span style="color: #8b0000">mesh2heightfield</span>: new tool to convert a mesh file into a 2D height map (from a normal direction N and from a starting point P). 
 * <span style="color: #00008b">ofs2off</span>: convert OFS mesh format towards a OFF variant. 
 * <span style="color: #00008b"> raw2HDF5</span>: convert raw image to HDF5. 
 * <span style="color: #00008b">raw2vol</span> and <span style="color: #00008b">vol2raw</span>: transform 3D volumes files from (resp. to) raw to vol. 
 * <span style="color: #00008b"> sdp2vol</span>: a simple tool to create a 3d vol image from 3d digital points. 
 * <span style="color: #00008b">slice2vol</span>: tool to merge slices into one 3d volumic file. 
 * <span style="color: #8b0000">vol2heightfield</span>: a new tool to transform volumetric file into 2D heightmap. 
 * <span style="color: #00008b">vol2obj</span>: convert a volume file into OBJ format (all voxels belonging to threshold interval) 
 * <span style="color: #00008b">vol2raw</span>: convert a vol to a 8-bit raw file. 
 * <span style="color: #00008b"><span style="color: #00008b">vol2sdp</span><span style="font-size: 16px">: a simple tools to extract digital points from 3d vol files.</span></span> 
 * <span style="color: #00008b"> vol2slice</span>: tool to extract all slices from 3d volumic images. 
 * <span style="color: #8b0000">volAddNoise</span>: a new tool to add noise (Kanungo's) to a binary 3D object. 
 * <span style="color: #00008b"> volBoundary2obj</span>: a simple tool to export the boundary of a an object in a volumetric file to OBJ. 

* **<span style="color: #00008b">distanceTransform/</span>**: 
 * <span style="color: #00008b">LUTBasedNSDistanceTransform</span>: Compute the 2D translated neighborhood-sequence distance transform of a binary imag 
 * <span style="color: #00008b"> CumulativeSequenceTest</span> and <span style="color: #00008b">RationalBeattySequenceTest</span>: tests from LUTBasedNSDistanceTransform. 

* **estimators/**: 
 * <span style="color: #00008b">2dLocalEstimators</span>: program to compare local curvature/tangent estimators on implicit shapes: 
   * Maximal DSS based estimators 
   * Maximal DCA based estimators 
   * Binomial convolver based estimators 
   * Integral Invariants based estimators 
 * <span style="color: #00008b">3dLocalEstimators</span>: program to compare 3D local curvature estimators  (mean, gaussian and principal curvatures) on 3D implicit shapes  with integral invariant and monge via jet fitting (with also noise robustness measure). 
 * <span style="color: #00008b">curvatureBC</span>: curvature estimator using the Binomial convolver. 
 * <span style="color: #00008b">curvatureMCMS</span>: curvature estimator using the maximal segments cover (to be updated for current DGtal version). 
 * <span style="color: #00008b">curvatureScaleSpaceBCC</span>: a tool to display the curvature scale space of a given contour with the Binomial Convolver Curvature Estimator. 
 * <span style="color: #00008b"> euleurCharacteristic </span>: bruteforce tool to extract (volumetric) Euler characteristic from volumetric binary object. 
 * <span style="color: #00008b">lengthEstimator</span>: program to generate multigrid analysis of length estimators. 
 * <span style="color: #00008b"> generic3dNormalEstimators</span>: Computes a normal vector field over a digitized 3D implicit surface for several estimators (II|VCM|Trivial|True). 
 * <span style="color: #00008b">statisticsEstimators</span>: compute satistics (L1, L2, Loo) from results of two estimators. 
 * <span style="color: #00008b">tangentBC</span>: tangent estimator using the Binomial convolver. 
 * <span style="color: #00008b">vol2normalField</span>: compute the normal vector field of a given vol file . 

* **shapeGenerator/**: 
 * <span style="color: #00008b">shapeGenerator</span>: generate multigrid shape 
 * <span style="color: #00008b">contourGenerator</span>: generate multigrid shape contours 

* **visualization/**: 
 * <span style="color: #00008b">3dCompSurfelData</span>: a tool to compare generic surfel data informations given from two data files.
 * <span style="color: #00008b"> <span style="color: #008b00">3dCurvatureViewer</span></span>: permits to compute and visualize mean or gaussian curvature and principal curvature directions of  binary shape. 
 * <span style="color: #00008b"> <span style="color: #008b00">3dCurvatureViewerNoise</span></span>: same as 3dCurvatureViewer, but allows to add some noise to objects. 
 * <span style="color: #00008b">3dCurveViewer</span>: A tool for visualizing the tangential cover of 3d curves. 
 * <span style="color: #00008b">3dDisplaySurfelData</span>: display surfel data from SDP file with color attributes given as scalar interpreted as color. 
 * <span style="color: #00008b">3dHeightMapViewer</span>: display a 2D image as heightmap by using QGLviewer. 
 * <span style="color: #00008b"> <span style="color: #008b00">3dImageViewer</span></span>: new tool to display slice image with interactive translatations or rotations (can open dicom format if WITH_ITK is set to true). 
 * <span style="color: #00008b">3dSDPViewer</span>: basic display of a sequence of 3d points (as voxel or sphere) and vectors by using QGLviewer. 
 * <span style="color: #00008b">3dVolBoundaryViewer</span>: Display the boundary of a volume file by using QGLviewer. 
 * <span style="color: #00008b">3dVolViewer</span>: volume file (.vol and .pgm3d) viewer with QGLViewer. 
 * <span style="color: #00008b">displayContours</span>: display discrete contours from various format (.fc (freemanchain), .sdp). 
 * <span style="color: #00008b"> <span style="color: #008b00">meshViewer</span></span>: display 3D mesh from OFS or OFF format. 
 * <span style="color: #00008b">patternTriangulation</span>: a new tool that draws with Board2D the convex hull, the closest-point Delaunay triangulation or the farthest-point Delaunay triangulation of a pattern. 
 * <span style="color: #00008b"> <span style="color: #008b00">sliceViewer</span></span>: a new 2D and 3D slice viewer from 3D volumic files ( pgm3d, vol, longvol, and DICOM with ITK). 
 
* **volumetric/**: 
  * <span style="color: #00008b">3dVolMarchingCubes</span>: marching cubes form a Vol file 
  * <span style="color: #00008b">homotopicThinning3D</span>: ultimate skeleton from vol file 
  * <span style="color: #00008b">volAddBorder</span>: add a 1 voxel boundary with value 0 to a vol file. 
  * <span style="color: #00008b">volCComponentCounter</span>: a simple program to count the number of connected components in a 3D image. 
  * <span style="color: #00008b">volCrop</span>: crop an 3D vol image from to points. 
  * <span style="color: #00008b">volFlip</span>: tool to flip all volume slice images according a given dimension. 
  * <span style="color: #00008b">volImageMetrics</span>: apply basic measures from two volumetric images: RMSE and PSNR. 
  * <span style="color: #8b0000">volIntensityScale</span>: a simple tool to apply a linear scale of the intensity given in a volumetric file. 
  * <span style="color: #00008b">volReSample</span>: apply a basic re sampling of a 3D volumetric image (.vol, .longvol, .pgm3d) with a given grid size. 
  * <span style="color: #00008b">volSegment</span>: Segment volumetric file from a simple threshold which can be set automatically from the otsu estimation. 
  * <span style="color: #00008b">volShapeMetrics</span>: apply shape measures for comparing two volumetric images A and B (shape defined from thresholds) 
  * <span style="color: #00008b">volSubSample</span>: sub sample a vol file (division by 2 in each direction) 
  * Measures from voxel partition (true/false+-, precision recall, f-measure) 
  * Measures bases on euclidean distance between the two Shape A and B. 
  * <span style="color: #00008b">volTrValues</span>: a basic tool to transform the voxel values from an input/output set.

### How to get and install DGtalTools 

You can get the DGtalTools by using git:

```git clone git://github.com/DGtal-team/DGtalTools.git``` or the source archive: [DGtalTools-0.8-Source.tar.gz][4] 

Installation: 
* use cmake tool to generate a build script (MakeFile, VS project,..) from the CMakeLists.txt 
* DGtal must be installed in your system. Concerning DGtal dependencies (boost, Qt,...), all the dependencies used to compile your DGtal library must be present to build the DGtalTools.

 [1]: http://github.com/DGtal-team/DGtalTools
 [2]: http://www.ipol.im
 [3]: http://dgtal.org/doc/stable/packageTutorials.html
 [4]: http://dgtal.org/wp/wp-content/uploads/2012/06/DGtalTools-0.8-Source.tar.gz
