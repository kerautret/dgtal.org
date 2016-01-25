---
ID: 261
post_title: For users
author:
  - 'a:1:{i:0;s:34:"a:1:{i:0;s:16:"David Coeurjolly";}";}'
post_date:
  - 'a:1:{i:0;s:37:"a:1:{i:0;s:19:"2011-07-29 18:31:23";}";}'
post_excerpt:
  - 'a:1:{i:0;s:17:"a:1:{i:0;s:0:"";}";}'
layout: page
permalink:
  - 'a:1:{i:0;s:29:"a:1:{i:0;s:11:"/for-users/";}";}'
published: true
gr_overridden:
  - 'a:1:{i:0;s:36:"a:1:{i:0;s:18:"a:1:{i:0;s:1:"0";}";}";}'
---
To use DGtal in your own project, a very nice solution exists with *cmake*: here you have an example to build a DGtal *helloword*: <code lang="cmake">
PROJECT(Helloworld)
##Required in DGtal
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
FIND_PACKAGE(DGtal REQUIRED)
INCLUDE_DIRECTORIES(${DGTAL_INCLUDE_DIRS})
LINK_DIRECTORIES(${DGTAL_LIBRARY_DIRS})

ADD_EXECUTABLE(helloworld helloworld)
TARGET_LINK_LIBRARIES(helloworld ${DGTAL_LIBRARIES})
</code>

See the [documentation][1] for details. DGtal is a free-software (Lesser Gnu Privacy License - LGPL) so you can freely use it and distribute it. However, if you use DGtal in your own project, we would be pleased to be kept in touch. If you want to refer to DGtal in your publications, please use the following bibtex entry:

<code lang="bibtex">@Misc{DGtal,
title = {{D}{G}tal: Digital Geometry tools and algorithms library},
note = {\url{http://dgtal.org}}
}</code>
## Projects/Publications using DGtal

* ANR Grant [digitalSnow][2] (ANR-11-BS02-009) "Digital Geometry and Applied Mathematics for Snow Metamorphism"
* Longuetaud, F.; Mothe, F.; Kerautret, B.; Krähenbühl, A.; Hory, L.; Leban, J. & Debled-Rennesson, I. Automatic knot detection and measurements from X-ray CT images of wood: A review and validation of an improved algorithm on softwood samples.
* Computers and Electronics in Agriculture, 2012, 85, 77-89
* Kowalczyk, M. K.; Kerautret, B.; Naegel, B. & Weber, J.,Revisiting Component Tree Based Segmentation Using Meaningful Photometric Informations. *Proc of International Conference ICCVG, Springer, 2012, 7594, 475-482*

 [1]: http://dgtal.org/doc/stable/moduleHowToUseDGtal.html
 [2]: http://liris.cnrs.fr/dsnow
