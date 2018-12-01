HAAR Casacada 

Install Opencv 

---------------------------

MASK RCNN INSTALL this requirement 

numpy
scipy
cython
h5py
Pillow
scikit-image
tensorflow-gpu==1.5
keras
jupyter
numpy
scipy
Pillow
cython
matplotlib
scikit-image
tensorflow>=1.3.0
keras>=2.0.8
opencv-python
h5py
imgaug
IPython[all]

Instanll Virtual Envoriment 
active venv
---
activate MaskRCNN - opencv2 , numpy 
Create a conda virtual environment¶
we will be using Anaconda with python 3.6.

If you don't have Anaconda, follow this tutorial

https://www.youtube.com/watch?v=T8wK5loXkXg
run this command in a CMD window
conda create -n MaskRCNN python=3.6 pip
---------------


Install 
Cuda 9.0 Not 10 , 10 will not working 

CudNN 7.3 NVDIa Developer 


https://medium.com/@minhplayer95/how-to-install-tensorflow-with-gpu-support-on-windows-10-with-anaconda-4e80a8beaaf0

https://www.pugetsystems.com/labs/hpc/The-Best-Way-to-Install-TensorFlow-with-GPU-Support-on-Windows-10-Without-Installing-CUDA-1187/


https://github.com/tensorflow/tensorflow/issues/18652

----------------
 Install pycocotools¶
NOTE: pycocotools requires Visual C++ 2015 Build Tools
download here if needed https://www.visualstudio.com/downloads/#build-tools-for-visual-studio-2017

clone this repo

git clone https://github.com/philferriere/cocoapi.git
use pip to install pycocotools
pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI



----

Training Dataset 
Downloading dataset from http://cocodataset.org/#download 2017 Train images [118K/18GB]
and annotation  Train/Val annotations [241MB]
2014 Train images [83K/13GB]
2014 Val images [41K/6GB]
2014 Test images [41K/6GB]

Dataset have three part
First Training Data
Secound Validataion Data
Third Test Data 
Each Part IS VERY IMPORTANT 
Download file instances_valminusminival2014.json add it into Anntotation folder 

https://drive.google.com/drive/folders/0B1_fAEgxdnvJSmF3YUlZcHFqWTQ

and file 

instances_minival2014 on google add it into Anntotation folder 



Extrac annotation in COCO Folder

Run command 
python samples/coco/coco.py train --dataset=/path/to/coco/ --model=coco with preweight from COCO

python coco.py train --dataset=../coco/ --model=coco


----

Run File 

process_video.py

capture = cv2.VideoCapture('bear.mp4')
  
Change it to your video 


Some ERRORS I have

---
https://medium.com/@minhplayer95/how-to-install-tensorflow-with-gpu-support-on-windows-10-with-anaconda-4e80a8beaaf0

https://www.pugetsystems.com/labs/hpc/The-Best-Way-to-Install-TensorFlow-with-GPU-Support-on-Windows-10-Without-Installing-CUDA-1187/

https://github.com/tensorflow/tensorflow/issues/18652

https://github.com/cocodataset/cocoapi/issues/9
https://github.com/tensorflow/models/issues/4864
---

