# Real-time Hand Sign detection using TensorFlow Object Detection API
An end-to-end implementation of training and leveraging our own custom object detection model using the tensorflow object detection API.

<kbd>
<img src="https://user-images.githubusercontent.com/29462447/116663374-a1482780-a9b4-11eb-903e-aa3a22680d4d.jpg" data-canonical-src="https://user-images.githubusercontent.com/29462447/116663374-a1482780-a9b4-11eb-903e-aa3a22680d4d.jpg"/> 
</kbd>

&nbsp;
## Installation and Usage:
## Steps
<br />
<b>Step 1.</b> Clone this repository: https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API.git
<br/><br/>
<b>Step 2.</b> Create a new virtual environment 
<pre>
python -m venv env
</pre> 
<br/>
<b>Step 3.</b> Activate your virtual environment
<pre>
source tfod/bin/activate # Linux
.\tfod\Scripts\activate # Windows 
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=env
</pre>
<br/>
<b>Step 5.</b> Collect images using the Notebook <a href="https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API/blob/main/Image%20Collection.ipynb">1. Image Collection.ipynb</a> - ensure you change the kernel to the virtual environment as shown below
<img src="https://i.imgur.com/8yac6Xl.png"> 
<br/>
<b>Step 6.</b> Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the two folders - train and test.<br/>
<br/><br/>
<b>Step 7.</b> Begin training process by opening <a href="https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API/blob/main/Training%20%26%20Detection.ipynb">2. Training and Detection.ipynb</a>, this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model. 
<br /><br/>
<b>Step 8.</b> During this process the Notebook will install Tensorflow Object Detection. You should ideally receive a notification indicating that the API has installed successfully at Step 8 with the last line stating OK.  
<img src="https://i.imgur.com/FSQFo16.png">
If not, resolve installation errors by referring to the <a href="https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API/blob/main/Error%20Guide.md">Error Guide.md</a> in this folder.
<br /> <br/>
<b>Step 9.</b> Once you get to step 6. Train the model, inside of the notebook, you may choose to train the model from within the notebook. I have noticed however that training inside of a separate terminal on a Windows machine you're able to display live loss metrics. 
<img src="https://i.imgur.com/K0wLO57.png"> 
<br />
<b>Step 10.</b> You can optionally evaluate your model inside of Tensorboard. Once the model has been trained and you have run the evaluation command under Step 7. Navigate to the evaluation folder for your trained model e.g. 
<pre> cd Tensorlfow/workspace/models/my_ssd_mobnet/eval</pre> 
and open Tensorboard with the following command
<pre>tensorboard --logdir=. </pre>
Tensorboard will be accessible through your browser and you will be able to see metrics including mAP - mean Average Precision, and Recall.
<br />
