# OpenCv-TensorFlow-Pose-Estimation-on-Videos.-Colab-
OpenCv + TensorFlow Pose Estimation on Videos

"""
OpenCv + TensorFlow Pose Estimation on Videos. [Colab]
"""

NOTE:

The following packages were installed on colab, you can install then on your 
local machine by removing (!) mark. 
Also, remember to change the drive directory path on colab and, or local methods.

Example: <br>
`%cd /content/drive/My Drive/tf-pose-estimation`

In the above code block, my Google Drive is mounted as (`drive`).
After a successful mount, i extracted `tf-pose-estimation` to the drive relative path as 
shown in the code block.

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

*Note:*
This code block is run in the main file, run once and comment the code blocks

