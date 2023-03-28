<!-- Banner -->
<p align="center">
  <a href="https://www.bosch.com.vn/" title="Bosch Global Software Technologies" style="border: none;">
    <img src="images/banner_aiteam.png" alt="Bosch Global Software Technologies"> 
  </a>
</p>

<h3 align="center"><b>FIT.Fest'23</b></h3>
<h3 align="center"><b>Future.Innovation.Technology</b></h3>
<h1 align="center"><font color=""><b>Master Class</b></font></h1>

# Introduction
In this repository, we provide our source code for 2 topic License Plate Recognition and Self-parking Car. We also have mandatory to guild implement our experiment step by step.


* [License Plate Recognition](#LicensePlateRecognition)
* [Self-parking Car](#Self-parking-(Car))

# License Plate Recognition
In 'LicensePlateRecognition' folder, please clone [yolov5](https://github.com/ultralytics/yolov5) repository on github due to this topic we strongly base on this detection method.

```
cd ./LicensePlateRecognition/
git clone https://github.com/ultralytics/yolov5.git
```

Next step, move our config file that we prepared for training model ( yolov5_carPlate.yaml ) to data folder or use this command.

```
mv yolov5_carPlate.yaml ./yolov5/data/yolov5_carPlate.yaml
```

```
MasterClass_FITFest2023/
   |________Self-parkingCar/
   |________LicensePlateRecognition/
               |_data/
                  |_ yolov5_carPlate.yaml

```
After that, please check [ALPR.ipynb](https://github.com/nguyenttkn/MasterClass_FITFest2023/blob/main/LicensePlateRecognition/ALPR.ipynb) for full documentation on training, testing and deployment step by step.

# Self-parking Car

Download all material for this topic at this [link](https://bosch-my.sharepoint.com/:u:/p/thg5hc/EWYdsIbUr6RBkakb6GcVogMB-OsINT-r9OacCOdxuGwpug?e=eSU7vi)

<details> 
  <summary><b>Install the mlagents library</b></summary><br/>

```
pip install ml-agents
```

<p align="center">
  <img src="./images/mlagents.png" width="75%" title="Install_mlagents">
</p>

</details>

<details> 
  <summary><b>Install UnityHub and Unity Editor</b></summary><br/>

Next step, please use this  [link](https://unity.com/download) to install UnityHub and then install Unity Editor via UnityHub. 


<p align="center">
  <img src="./images/unityhub.png" width="75%" title="Install_mlagents">
</p>

Use the Unity Editor to open the project we have provided, to make sure everything works, please check the ML-Agents package in PackageManagement to see if it is already installed

<p align="center">
  <img src="./images/package.png" width="75%" title="Install_mlagents">
</p>

Take a look to our environment. 

<p align="center">
  <img src="./images/example.png" width="75%" title="Example">
</p>

</details>

<details> 
  <summary><b>Training model</b></summary><br/>


```
mlagents-learn trainner_settings.yaml --run-id='AITeam_FitFest2023'
```



