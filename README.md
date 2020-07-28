# OpenCv-TensorFlow-Pose-Estimation-on-Videos.-Colab-
OpenCv + TensorFlow Pose Estimation on Videos

### ==================Project Description======================================
"""
OpenCv + TensorFlow Pose Estimation on Videos. [Colab]
"""

NOTE:

The following packages were installed on colab, you can install then on your 
local machine by removing (!) mark. 
Also, remember to change the drive directory path on colab and, or local methods.

Example: <br>
`%cd /content/drive/My Drive/tf-pose-estimation`


Install the following packages;

# Install tensorflow version 1.14.0

!pip3 install tensorflow==1.14.0

!git clone https://github.com/ildoonet/tf-pose-estimation.git > /dev/null

%cd /content/drive/My Drive/tf-pose-estimation

!pip3 -q install -r requirements.txt

!python3 setup.py install

!wget https://www.dropbox.com/s/nf7ffqjv37dvin0/graph_opt.pb?dl=0 -O ./models/graph/cmu/graph_opt.pb 

!sudo apt install swig

%cd tf_pose/pafprocess

!swig -python -c++ pafprocess.i && python3 setup.py build_ext --inplace

%cd /content/drive/My Drive/tf-pose-estimation


### ==================Project Description End==================================
