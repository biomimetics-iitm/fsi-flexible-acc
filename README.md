# fsi-flexible-acc
This code simulates the fluid-structure interaction of a fully flexible filament immeresd in uniform flow. Plunge and pitch actuation can be provided at the leading edge of the filament.

To run on a cluster (e.g. in the synchrony cluster available in the Biomemetics and Dynamic Lab IIT Madras, India):

// First load the GPU module using following command in terminal//

module load nvhpc/20.7

// Compile the souce_code //

pgc++ -o make.out -acc -Minfo=accel -ta=tesla:cc80 source_code.cpp


// Submit the code for simulation using run_IBMFSI.cmd //

qsub run_IBMFSI.cmd


## Citation

1. [Capturing the dynamical transitions in the flow-field of a flapping foil using Immersed Boundary Method](https://www.sciencedirect.com/science/article/abs/pii/S0889974620300128)
```
@article{majumdar2020capturing,
  title={Capturing the dynamical transitions in the flow-field of a flapping foil using Immersed Boundary Method},
  author={Majumdar, Dipanjan and Bose, Chandan and Sarkar, Sunetra},
  journal={Journal of Fluids and Structures},
  volume={95},
  pages={102999},
  year={2020},
  publisher={Elsevier}
}
```
2. [Performance Enhancement of an Immersed Boundary Method Based FSI Solver Using OpenMP](https://www.nal.res.in/cfdimgs/FullPaper/P27-Performance%20Enhancement%20of%20an%20Immersed%20Boundary%20Method.pdf)

```
@article{shahperformance,
  title={Performance Enhancement of an Immersed Boundary Method Based FSI Solver Using OpenMP},
  author={Shah, Chhote Lal and Majumdar, Dipanjan and Sarkar, Sunetra}
}
```
3. [Massive parallelisation and performance enhancement of an immersed boundary method based unsteady flow solver](https://arxiv.org/abs/2402.17337)

```
@inproceedings{sundar2022massive,
title={Massive parallelisation and performance enhancement of an immersed boundary method based unsteady flow solver},
author={Sundar, Rahul and Majumdar, Dipanjan and Shah, Chhote Lal and Sarkar, Sunetra},
booktitle={9th International and 49th National Conference on Fluid Mechanics and Fluid Power, IIT Roorkee, India},
year={2022}
}
```
