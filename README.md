# MPM-Particle-Generator

The generator allows to create numerical MPM models based on the contour lines of the land. It has three main characteristics: 

- the construction of the MPM discrete model is based only on raster digital elevation model (DEM) data;
- finite element meshes are not required;
- the heterogeneities are defined by the DEM data of each material;

![Alt text](examples/workflow/workflow.png?raw=true "Workflow of the MPM-Generator")

# Compiling

The program can be compiled using an standard C++ compiler. To compile it using GCC compiler run the script in the compile-gcc directory:

```bash
compile-gcc/compile-gcc.sh
```

# Examples

There are two examples: A sine wave model and the Daguangbao Landslide model.

## The sine-wave example

The file input is located in the example folder:

```bash
examples/example-1-sinewave/sine-wave.dat
```

To run this model go to folder and run the generator:

```bash
mpm-generator sine-wave.dat
```

The mpm model of the Sine wave results in:

![Alt text](examples/example-1-sinewave/sine-wave-mpm-model.png?raw=true "Sine-wave mpm model")

## The Daguangbao Landslide example

The file input is located in the example folder:

```bash
examples/example-2-daguangbao/daguangbao.dat
```

To run this model go to folder and run the generator:

```bash
mpm-generator daguangbao.dat
```

The mpm model of the Daguangbao landslide results in:

![Alt text](examples/example-2-daguangbao/daguangbao-mpm-model.png?raw=true "Daguangbao mpm model")

## Results visualization

After the generator execute the input file a vtu file is created. This file can be loaded in ParaView in order to verify the model. 

# Reference

[A 3D discretization procedure for the material point method-MPM](https://doi.org/10.1007/s40571-019-00303-7)

# Cite this code as

Fernández, F., do Amaral Vargas, E. & Quadros Velloso, R. A 3D discretization procedure for the material point method (MPM). Comp. Part. Mech. 7, 725–733 (2020). https://doi.org/10.1007/s40571-019-00303-7
