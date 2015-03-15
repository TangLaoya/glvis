[![](http://images.glvis.googlecode.com/hg/metatron-logo.png)](http://code.google.com/p/glvis/wiki/Gallery)
<a href='Hidden comment: 
http://glvis.googlecode.com/files/metatron.png
'></a>

## Introduction ##
GLVis is an OpenGL tool for _accurate_ visualization of _serial_ and _parallel_ finite element meshes and grid functions.

## Latest release ##
### [glvis-3.0.tgz](http://goo.gl/S1qFfw) | [Code documentation](http://doxygen.glvis.googlecode.com/hg/html/index.html) | [New features](http://glvis.googlecode.com/hg/CHANGELOG) ###

_While we recommend that users download the latest release above, all GLVis releases are available [here](Releases.md). Please use the [issue tracker](http://code.google.com/p/glvis/issues) to report [bugs](http://code.google.com/p/glvis/issues/entry?template=Defect%20report%20from%20user) or post [questions or comments](http://code.google.com/p/glvis/issues/entry?template=Question%20or%20Comment)._

## Overview ##
When started without any options, GLVis [establishes a server](http://code.google.com/p/glvis/wiki/OptionsAndUse#Server_mode), which waits for socket connections and visualizes any received data in a separate interactive window. This allows for the results of simulations run on a remote (parallel) machine to be visualized on the local user desktop, taking advantage of hardware OpenGL acceleration. GLVis originated from the previous research effort in the (unreleased) AggieFEM/aFEM project.

GLVis can be used to [visualize meshes](http://code.google.com/p/glvis/wiki/OptionsAndUse#Visualizing_meshes) and a wide variety of [finite element grid functions](http://code.google.com/p/glvis/wiki/OptionsAndUse#Visualizing_functions), including arbitrary high-order finite element and NURBS solutions. It can run a [batch sequence of commands](http://code.google.com/p/glvis/wiki/OptionsAndUse#GLVis_scripts) (GLVis scripts), or display [previously saved socket streams](http://code.google.com/p/glvis/wiki/OptionsAndUse#Server_mode).

GLVis is based on the modular finite element methods library [MFEM](http://mfem.googlecode.com), which supports in particular general [curvilinear](http://code.google.com/p/glvis/wiki/MeshFormats) and [NURBS](http://code.google.com/p/glvis/wiki/NURBS) meshes, input in [unstructured VTK mesh format](http://code.google.com/p/glvis/wiki/CurvilinearVTKMeshes) and the visualization of parallel meshes and solutions (either saved in separate files or sent by separate socket connections from each processor). Some examples of its use can be found in the [Gallery](http://code.google.com/p/glvis/wiki/Gallery) page.

Though depending on MFEM for its finite element dictionary, GLVis can be used independently for parallel and serial visualization. For example, the _[hypre](http://www.llnl.gov/casc/hypre)_ library includes scripts for displaying the numerical results from its parallel example codes through GLVis.

## Examples ##
  * Start a socket server: **`glvis`**
  * View a mesh: **`glvis -m star.mesh`**
  * View a mesh with a finite element grid function: **`glvis -m star.mesh -g sol.gf`**
  * View mesh and solution from a run on 4 processors: **`glvis -np 4 -m mesh -g sol`** (assuming data saved in files: `mesh.000000`, ... , `mesh.000003` and `sol.000000`, ...  , `sol.000003`)
  * Use **`glvis -h`** to get help on all command line options.
  * See [README](http://glvis.googlecode.com/hg/README) for a detail of the keystroke commands accepted in the GLVis interactive window.

## Tutorials ##
  * [Building](http://code.google.com/p/mfem/wiki/Building?ts=1303074759&updated=Building#Details)
  * [Command-line options and general use](http://code.google.com/p/glvis/wiki/OptionsAndUse)
  * [Mesh formats](http://code.google.com/p/glvis/wiki/MeshFormats)
  * [Parallel visualization](http://code.google.com/p/glvis/wiki/ParallelVisualization)
  * [Curvilinear VTK meshes](http://code.google.com/p/glvis/wiki/CurvilinearVTKMeshes)
  * [NURBS meshes and solutions](http://code.google.com/p/glvis/wiki/NURBS)
  * [MFEM tutorials](http://code.google.com/p/mfem/wiki)