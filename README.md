# Real-time Hand Sign detection using TensorFlow Object Detection API 👍 👎 👌✌️👐
![tensorflow-logo](https://user-images.githubusercontent.com/29462447/116670987-094f3b80-a9be-11eb-8ec8-f676ef5b94e5.png)
### An end-to-end implementation of training and leveraging our own custom object detection model using the tensorflow object detection API.
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
<b>Step 5.</b> Collect images using the Notebook <a href="https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API/blob/main/Image%20Collection.ipynb">1. Image Collection.ipynb</a> - ensure you change the kernel to the virtual environment as shown:
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/116665184-10268000-a9b7-11eb-94d7-991321e850d3.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/116665184-10268000-a9b7-11eb-94d7-991321e850d3.png"/> 
</kbd>

&nbsp;
<br/>
<b>Step 6.</b> Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the two folders - train and test.<br/>
<br/><br/>
<b>Step 7.</b> Begin training process by opening <a href="https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API/blob/main/Training%20%26%20Detection.ipynb">2. Training and Detection.ipynb</a>, this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model. 
<br /><br/>
<b>Step 8.</b> During this process the Notebook will install Tensorflow Object Detection. You should ideally receive a notification indicating that the API has installed successfully at Step 8 with the last line stating OK.  
<kbd>
<img src="https://i.imgur.com/FSQFo16.png" data-canonical-src="https://i.imgur.com/FSQFo16.png"/> 
</kbd>
&nbsp;
If not, resolve installation errors by referring to the <a href="https://github.com/prateekralhan/Hand-Sign-detection-using-TensorFlow-Object-Detection-API/blob/main/Error%20Guide.md">Error Guide.md</a> in this folder.
<br /> <br/>
<b>Step 9.</b> Once you get to step 6. Train the model, inside of the notebook, you may choose to train the model from within the notebook. I have noticed however that training inside of a separate terminal on a Windows machine you're able to display live loss metrics. 
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/116666186-4e706f00-a9b8-11eb-9c0f-a4b449ca2f35.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/116666186-4e706f00-a9b8-11eb-9c0f-a4b449ca2f35.png"/> 
</kbd>
&nbsp;
<br />
<b>Step 10.</b> You can optionally evaluate your model inside of Tensorboard. Once the model has been trained and you have run the evaluation command under Step 7. Navigate to the evaluation folder for your trained model e.g. 
<pre> cd Tensorlfow/workspace/models/my_ssd_mobnet/eval</pre> 
and open Tensorboard with the following command
<pre>tensorboard --logdir=. </pre>
Tensorboard will be accessible through your browser and you will be able to see metrics including mAP - mean Average Precision, and Recall.
<br />

<b>Training metrics:</b>
<p style="text-align:center"> 
  <kbd>
  <img src="https://user-images.githubusercontent.com/29462447/116665999-1406d200-a9b8-11eb-8f2c-435ec1453f0b.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/116665999-1406d200-a9b8-11eb-8f2c-435ec1453f0b.png"/> 
  </kbd>
  &nbsp;
</p>

<b>Evaluation metrics:</b>
<p style="text-align:center"> 
  <kbd>
  <img src="https://user-images.githubusercontent.com/29462447/116666450-955e6480-a9b8-11eb-995b-6bedb1a4d8c5.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/116666450-955e6480-a9b8-11eb-995b-6bedb1a4d8c5.png"/> 
  </kbd>
  &nbsp;

  <kbd>
  <img src="https://user-images.githubusercontent.com/29462447/116666446-94c5ce00-a9b8-11eb-9620-7c80a7b85781.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/116666446-94c5ce00-a9b8-11eb-9620-7c80a7b85781.png"/> 
  </kbd>
  &nbsp;
</p>

<b>Results</b>

![thumbsup](https://user-images.githubusercontent.com/29462447/116669982-d9ebff00-a9bc-11eb-9191-edb855372941.png)
![thumbsdown](https://user-images.githubusercontent.com/29462447/116669975-d8bad200-a9bc-11eb-88d1-733054554f93.png)
![thankyou](https://user-images.githubusercontent.com/29462447/116669968-d6587800-a9bc-11eb-8532-7168656d4519.png)
![livelong](https://user-images.githubusercontent.com/29462447/116669992-dce6ef80-a9bc-11eb-8963-eca65a517887.png)





