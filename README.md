# Simulation container
This container is defined in `simulation_container.def`.

The following packages are available in the container:
1. `EvtGen` (with `Tauola` and `Photos`)
2. `Rapidsim`
3. Root framework
4. `HepMC3`
5. `Pythia8`


In addition, the container also includes CUDA framework (11.8) as well cuDNN (8.6.0). However, these remain
untested. Until then, please use the Docker container provided by TensorFlow.

Installation of tensorflow and pytorch is purposefully omitted to allow user flexibility and local installation.
With all the requirements met, it should be straightforward to install them direcly via python3-pip.

## Building
To build the container you can issue the following command:
```
sudo singularity build simulation_container.sif simulation_container.def
```

## Running the container
```
singularity shell simulation_container.sif
```

## Pulling from DockerHub

Under works