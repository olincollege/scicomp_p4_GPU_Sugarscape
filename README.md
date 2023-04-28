## Project 4: Sugarscape Model with GPU Acceleration

This project is an attempt at an implementation of the Sugarscape model in Python with GPU acceleration using pyflameGPU2. The Sugarscape model is a simple model of an ecosystem of agents that interact with each other and with their environment to demonstrate the emeragance of economic inequality. The model is used to study a variety of phenomena, such as foraging, cooperation, and competition. The current version of the model does not work properly as the population seems to stay the same throught the trial. The model currently only implements metabolism differences between the agents. This model was heavily inspired and partially adapted from [Submodel Test](https://github.com/FLAMEGPU/FLAMEGPU2-submodel-benchmark/blob/master/src/main.cu#L40) from the official flame gpu documentation. 

## Getting Started

To get started with this project, you will need to install the following libraries:

* Python 3.6 or higher
* NumPy
* Matplotlib
* pyflameGPU2
* Cuda 11.2 or Older

Sure, here is a section about installing pyflamegpu:

## Installing pyflamegpu

To install pyflamegpu, you can use the following steps:

1. Install the following dependencies:
    * CMake >= 3.18
    * CUDA >= 11.0 and a Compute Capability >= 3.5 NVIDIA GPU
    * C++17 capable C++ compiler (host), compatible with the installed CUDA version (i.e VS2019+, or GCC >= 8.1)
    * git
    * Python >= 3.7 (optional)

2. Clone the pyflamegpu repository:

```
git clone https://github.com/FLAMEGPU/FLAMEGPU2
```

3. Change to the pyflamegpu directory:

```
cd FLAMEGPU2
```

4. Build pyflamegpu:

```
mkdir build
cd build
cmake ..
make -j$(nproc)
```

5. Install pyflamegpu:

```
make install
```

Once you have installed pyflamegpu, you can import it into Python using the following command:

```
import pyflamegpu
```

Once you have installed the required libraries, you can clone the github repository:

```
git clone https://github.com/olincollege/scicomp_p4_GPU_Sugarscape
```

The project directory contains a Jupyter notebook called `sugarscape.ipynb`. This notebook contains the code for the Sugarscape model. To run the code, open the notebook in Jupyter and select "Run" from the menu bar. The notebook contains a block of code that must be uncommented to download and install the library.

## Results

The model is not currently functional. The reasons are not fully obvious but it seems to be something to do with the Agent death and movement functions, in a real sugarscape model the population overtime should fluctuate, currently, as seen below, population remains constant.
![results](/pics/graph.PNG)
