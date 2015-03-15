GLVis is a _lightweight_ OpenGL tool for _accurate_ visualization of _serial_ and _parallel_ finite element meshes and functions. Its features include:
  * Accurate finite element mesh and function representation through interactive refinement.
  * [Server mode](https://code.google.com/p/glvis/wiki/OptionsAndUse#Server_mode) accepting multiple and/or persistent socket connections.
  * Support for triangular, quadrilateral, tetrahedral and hexahedral elements with [curved boundaries](https://code.google.com/p/glvis/wiki/MeshFormats#Curvilinear_and_more_general_meshes).
  * 2D and 3D, arbitrary high-order H1, H(curl), H(div), L2 and [NURBS](NURBS.md) elements.
  * Visualization of [parallel](http://code.google.com/p/glvis/wiki/ParallelVisualization) meshes and solutions.
  * ... and [many more](Features.md).

GLVis is based on the [MFEM](http://mfem.googlecode.com)  library and is currently used in the [BLAST](http://www.llnl.gov/casc/blast), _[hypre](http://www.llnl.gov/casc/hypre)_ and [XBraid](http://www.llnl.gov/casc/xbraid) projects. See also our [Gallery](Gallery.md).

## Latest Release ##
### [glvis-3.0.tgz](http://goo.gl/S1qFfw) | [User documentation](http://glvis.googlecode.com/hg/README) | [Code documentation](http://doxygen.glvis.googlecode.com/hg/html/index.html) | [New features](http://glvis.googlecode.com/hg/CHANGELOG) ###

_Please use the [issue tracker](http://code.google.com/p/glvis/issues) to report [bugs](http://code.google.com/p/glvis/issues/entry?template=Defect%20report%20from%20user) or post [questions or comments](http://code.google.com/p/glvis/issues/entry?template=Question%20or%20Comment)_. For older releases see [all releases](https://code.google.com/p/glvis/wiki/Releases).

## Documentation ##
The best starting point for new users is the [options and general use](http://code.google.com/p/glvis/wiki/OptionsAndUse) tutorial.

[Building](http://code.google.com/p/mfem/wiki/Building?ts=1303074759&updated=Building#Details) | [Mesh formats](http://code.google.com/p/glvis/wiki/MeshFormats) | [Parallel visualization](http://code.google.com/p/glvis/wiki/ParallelVisualization) | [VTK meshes](http://code.google.com/p/glvis/wiki/CurvilinearVTKMeshes) | [NURBS meshes and solutions](http://code.google.com/p/glvis/wiki/NURBS) | [MFEM tutorials](http://code.google.com/p/mfem/wiki)

GLVis is being developed at [CASC](http://computation.llnl.gov/casc/), [LLNL](https://www.llnl.gov/). It can be cited with
<pre>
@misc{glvis-tool,<br>
title = {{GLVis}: Accurate finite element visualization},<br>
howpublished = {\url{glvis.googlecode.com}}<br>
}</pre>
See also our list of [Publications](http://code.google.com/p/mfem/wiki/Publications).