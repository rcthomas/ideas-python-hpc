# Python in HPC 

Rollin Thomas, William Scullin, Matt Belhorn

Python's powerful elegance has driven its adoption at HPC centers for job
orchestration, visualization, exploratory data analysis, and even simulation.
But maximizing performance from Python applications can be challenging
especially on supercomputing architectures.  This webinar will explain those
challenges with a practical emphasis on using Python at NERSC, ALCF, and OLCF.
We will outline a variety of performance optimization strategies, tools for
measuring and addressing performance problems, and establish best practices for
Python in HPC.

[Registration](https://exascaleproject.org/event/python-in-hpc-2/)

# Outline

* Introduction
    * Motivate the talk
        * Demand for Python on supercomputers is growing
        * Python users need help adapting and achieving performance
    * Describe the scientific Python stack at a high level
    * Introduce theme: To achieve performance, identify and exploit parallelism

* Practical: Python at NERSC, ALCF, and OLCF
    * Use of software modules environment
    * Spack for on-site builds
    * Anaconda Python
    * Intel Distribution for Python
    * Customization methods available to users
        * virtualenv
        * conda environments
        * containers (Shifter)

* Using MPI to achieve multi-node performance
    * Overview of mpi4py
    * Caveats
        * about file system performance
        * about spawning/dynamic process control
    * Parallel I/O with h5py
    * Profiling analysis tools here (anyone use any with Python?)

* Using threads and vectorization for single-node performance
    * Threaded libraries (MKL, OpenMP) backing numpy, scipy
    * Performance tools like numexpr or numba
    * Cython
    * Writing C extensions
    * Profiling tools
        * Intel VTune for Python
        * cProfile and snakeviz
    * Alternative interpreters (PyPy?)


# Supplementary Materials

- [SC2016 Slides](https://github.com/ContinuumIO/supercomputing2016-python)
- NERSC Data Day Slides (No public link)
- [Scripts and examples for deploying python on OLCF resources](https://code.ornl.gov/m9b/nccs_python_reference).
- [Managing Python environments at the OLCF (slides)][external_materials/python_management.pdf]
