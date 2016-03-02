# deepdreamer-touchdesigner

**Deep dream with [caffe](http://caffe.berkeleyvision.org/) and [Touchdesigner](http://www.derivative.ca/)**

![CaptureDream](http://aledel.github.io/deepdreamer-touchdesigner/images/dreamtouch.jpg)

## Requirements
python 3.3.5
I use "anaconda" to be sure I have the most dependencies.
TouchDesigner currently uses python 3.3.6 but work with python 3.3.5

## Setup python with Anaconda

Install [anaconda](https://www.continuum.io/downloads) or [miniconda](http://conda.pydata.org/miniconda.html)
create a new environment called py33.
```
conda create -n py33 anaconda python=3.3.*
conda info --envs
activate py33
```
Ensure that there is the correct path in the system environment variable "path".
_path\to\anaconda\envs\py33_ and
_path\to\anaconda\envs\py33\scripts_

install protobuf
```
pip install protobuf==3.0.0b
```

## Install caffe module
you only need to add the path to the folder "python Caffe" to the system variable "PYTHONPATH"

## Config Touchdesigner
* in preferences, Python module path add path to *path/to/Anaconda/envs/py33/Lib/site-packages*.
* Touchdesigner use numpy 7 but caffe need version 9
  * **delete or move files and folders** numpy off *C:\Program Files\Derivative\TouchDesigner088\bin\Lib\site-packages* folder.

