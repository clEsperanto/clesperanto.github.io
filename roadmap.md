This document is under construction. 
Nothing is nailed in stone. 
Please commit changes, send pull-requests or create issues.

Let's make this a truly community-driven project by writing the roadmap together.


# Roadmap clEsperanto
## Mission 
Mission of the clEsperanto project is to unite sub-communities of scientific image analysis by bridging between 
programming languages and environments. 

1. We aim crafting an easily accessible image processing library.
2. We aim making image processing accessible for
   1. beginners and experts,
   2. programmers of any major language,
   3. users of any major operating system and
   4. owners of any major CPU and GPU hardware.
3. We aim writing easy to read, maintain and extend code.
4. We aim documenting our platform in an easily accessible way.
5. We aim forming a community where users and developers make decisions together.

# Tasks
To achieve our goals, we plan to adapt the [CLIJ](https://clij.github.io/) project to be accessible to a 
broader audience.

## Major tasks
1. Core development; at least two alternatives:
   1. Translating [ClearCL](https://github.com/clij/clij-clearcl) to either C++ and wrapping from Python/Java/...
   2. Translating ClearCL to Python/... (by exploiting e.g. [PyOpenCL](https://pypi.org/project/pyopencl/) and/or [gputools](https://github.com/maweigert/gputools)) and ensuring that all platforms do the same
2. API design
   1. Determining if the CLIJ2 API is generic enough to be accessible from all platforms / if code can be copy-pasted between languages.
   2. Finding ways for language specific [auto-generating APIs like in CLIJ2](https://github.com/clij/clij2-code-generators/blob/master/src/test/java/net/haesleinhuepf/clijx/codegenerator/OpGenerator.java). 
2. Wrapper development
   1. Java
   2. Python
   3. Macro
   4. C++
   5. ITK
3. User-documentation
   1. Introductory, partly generic, partly language specific
   2. Examples for all languages (Example generator?)
   3. [Documentation generator as in CLIJ2](https://github.com/clij/clij2-code-generators/blob/master/src/test/java/net/haesleinhuepf/clijx/codegenerator/DocumentationGenerator.java).
4. Testing
   1. Automated tests for all platforms
   2. Integration tests, manual user-experience tests
   3. Cross-language testing

## Target platforms
1. Operating Systems
   1. Windows 10
   2. MacOS
   3. Ubuntu Linux
2. Programming languages
   1. ImageJ Macro
   2. Fiji Jython
   3. Python
   4. Java
   5. Matlab
   6. Icy JavaScript
   7. C++
   8. Fiji Groovy
3. Hardware (OpenCL version > 1.2)
   1. Intel HD GPUs
   2. NVidia GTX/RTX
   3. AMD GPUs (Vega)

## Timeline

June 2020: Core development start

September 2020: Java/Pythong wrappers development start

December 2020: Core is functional, major wrapper code done.

February 2021: Alpha release of a minimal set of functions running on all target platforms and GPU hardware.

May 2021: Beta-release of full functionality

June 2021: Release of version 1.0. Code freeze to prevent breaking backwards compatibility

July 2021: Discussion of achievements and making a plan for version 2.0

## Potential future extensions
CUDA support?
