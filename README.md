# pybind11 example

This repo has a basic example of using pybind11 from CMake.

More details are available from [here](https://hopstorawpointers.blogspot.com/2018/06/using-c-code-from-python-with-pybind11.html)

Requirments:

  * CMake
  * pybind11 (v2.2 or higher)
  * gcc
  * python (and python-dev)

## Installing
 - `apt-get install cmake`
 - `virtualenv -p python test`
 - `source test/bin/activate'
 - `pip install "pybind11[global]"

To build you can do

```
mkdir build
cd build
cmake ..
make 
```

To run the python example code, from the `build` directory run:

```
PYTHONPATH=. python3 ../bindings.py
```

or directly from CMake run

```
make test
```
