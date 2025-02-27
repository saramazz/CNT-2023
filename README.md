# Computational Neuroscience Tutorial 2023
This tutorial has been designed for the following classes:
- 2022/2023 PhD class on Information Theory and Neural Modeling for Neural Engineering (Prof: Alberto Mazzoni), PhD Program in Biorobotics, Scuola Superiore Sant'Anna, Pisa
- 2021/2022 Master class on Biorobotics and Complex Systems (Prof: Alberto Mazzoni), Physics Degree, University of Pisa, Italy
- 2021/2022 PhD class on Information Theory and Neural Modeling for Neural Engineering (Prof: Alberto Mazzoni), PhD Program in Biorobotics, Scuola Superiore Sant'Anna, Pisa
- 2020/2021 PhD class on Large Scale Network Simulations, NeuroSchool PhD Program, INT, Marseille, France

## Introduction on Spiking Neural Networks (SNNs) by using PyNN language 

PyNN is a Python library for simulating neural networks. It provides a common interface for a variety of neural simulators, such as NEURON, NEST, and Brian, making it easy to switch between them without having to change the model code. PyNN allows users to define and simulate neural networks using a high-level, neuron-centric interface, similar to the way models are described in neuroscience literature. It is used in many research and education projects to study neural systems, and can be used to simulate models of the brain, as well as artificial neural networks.

## General PyNN [installation](http://neuralensemble.org/docs/PyNN/installation.html#installing-nest-and-pynest):
### PyNN and classic simulators
```
pip install <the-simulator> e.g. brain2, NEURON
pip install PyNN
```

### PyNN on the SpiNNaker neuromorphic system:

1. make the EBRAINS credentials to access the SpiNNaker server (https://spinn-20.cs.man.ac.uk/hub/login)
1. login on the Jupyter Lab interface
1. clone this repository `git clone https://github.com/albertoarturovergani/CNT-2023`
1. Open the directory `SpiNNaker/` and run the [CNT notebook](SpiNNaker/CNT_notebook.ipynb)

## Content:

### Overview for the design of Spiking Neural Networks (SNNs)

1. neurons
    - cell types
    - populations
    - recording variables
1. connections
    - synapse types
    - connections types
    - projections
3. simulation managing
    - computational settings
    - save and load outputs
    - visualization tools

### Tutorial notebook

- [CNT notebook](SpiNNaker/CNT_notebook.ipynb)

### Network examples 

- [entry network](SpiNNaker/eg_entry-network.ipynb)
- [decaying network](SpiNNaker/eg_decaying-network.ipynb)
- [persistent network](SpiNNaker/eg_persistent-network.ipynb)
- [diverging network](SpiNNaker/eg_diverging-network.ipynb)
- [small-world network](SpiNNaker/eg_small-world-network.ipynb)
- [testing cell models network](SpiNNaker/eg_testing-cell-models-network.ipynb)
- [testing STDP model network](SpiNNaker/eg_testing-STDP-model-network.ipynb)
- [VA_balance network](SpiNNaker/eg_balance-network.ipynb)

### Knowledge assumptions: 

- basis of spiking neural network theory (https://neuronaldynamics.epfl.ch/online/index.html) or (https://neuromatch.io/academy/)
- familiarity with physical quantities related to electric circuits (e.g., voltages, conductances, currents, etc)
- basic python coding (numpy, work with dictionaries, some matplotlib tools, etc)

### Expected take-home-points: 

- import the simulator
- setup the simulator
- decide the cell types 
- design the populations
- define the synapse types
- select the connection algorithm
- make the projections 
- idealize the stimulus
- run the simulation
- save the results
- recover the results
- postprocessing (visualization, statistics, etc)
- close the simulations

## Links
- [PyNN](http://neuralensemble.org/docs/PyNN/index.html)
- [SpiNNaker](http://apt.cs.manchester.ac.uk/projects/SpiNNaker/)
- [EBRAINS](https://ebrains.eu/)
- [The Human Brain Project](https://www.humanbrainproject.eu/en/)
