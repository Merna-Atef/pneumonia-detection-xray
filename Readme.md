<div id="top"></div>
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="">
    <img src="images/logo.png" alt="Logo" width="500" height="150">
  </a>

  <h2 align="center">Comparative Analysis of Deep Learning Models for Pneumonia Detection using X-ray Images</h2>
  <p align="center">
    This repo contains part of the work for the final project of Ultrasound Tissue Characterization Post-Grad course. This part of the project entails the detection of pneumonia from X-ray images.
  </p>
</div>

[![Contributors][contributors-shield]][contributors-url]


<!-- TABLE OF CONTENTS -->

## Table of Contents

  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#contribution">Contribution</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a>
      <ul>
        <li><a href="#data">Data Download</a></li>
        <li><a href="#notebooks">Notebooks</a></li>
      </ul>
    </li>
    <li><a href="#future">Future Work</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>





<div id="about-the-project"></div>

<!-- ABOUT THE PROJECT -->
## About the Project

We compare the usage of different well-known models for the binary classification task: **Pneumonia** vs **Healthy/Normal** in x-ray images.


<div id="contribution"></div>

<!-- Contribution -->
### Contribution
* **Data**
    * Combining **6** different datasets for X-ray images
    * Data augmentation
* **Models**
    * Usage of **7** different deep learning models architectures
    * VGG-16, VGG-19, InceptionV3, InceptionResnetV2, MobilenetV3, Resnet50, EfficientnetB3


<div id="built-with"></div>

<!-- Built-with -->
### Built-With
* [TensorFlow v2.7.0](https://www.tensorflow.org/install)
* [Python v3.9](https://www.python.org/)
* [Jupyter Lab](https://jupyter.org/)


<p align="right">(<a href="#top">back to top</a>)</p>


<div id="getting-started"></div>


<!-- GETTING STARTED -->
## Getting Started

The folder structure is as follows:
```
    ├── Original Data            # Github repos to the original data
    ├── Data                     # Combined datasets
        ├── test                 # Combined test data
            ├── normal
            ├── pneumonia 
        ├── train                # Combined train data
            ├── normal
            ├── pneumonia
        ├── train_augmented      # Combined augmented train data
            ├── normal
            ├── pneumonia
    ├── Notebooks                # Code Jupyter Notebooks
    └── README.md
```
<div id="prerequisites"></div>

### Prerequisites

* pydicom
  ```sh
  pip install pydicom
  ```
* matplotlib.pyplot
  ```sh
  pip install matplotlib
  ```
* numpy
  ```sh
  pip install numpy
  ```  
* Scikit-learn
  ```sh
  pip install sklearn
  ```  
 * OpenCV
  ```sh
  pip install open-cv
  ``` 


<div id="installation"></div>

### Installation

* Clone the repo
   ```sh
   git clone https://github.com/Merna-Atef/pneumonia-detection-xray.git
   ```
<p align="right">(<a href="#top">back to top</a>)</p>



<div id="usage"></div>


<!-- USAGE EXAMPLES -->
## Usage

This section discusses how to run the code and download all 6 datasets.

<div id="data"></div>

### Data Download
To download the 6 datasets: do as follows and place them in the folder `Original Data`
1. Clone **Chest X-ray** dataset from this github [link](https://github.com/ieee8023/covid-chestxray-dataset.git) into `Original Data` folder 

2. Download **RSNA Pneumonia Detection Challenge** dataset from this Kaggle [link](https://www.kaggle.com/c/rsna-pneumonia-detection-challenge) into `Original Data` folder and unzip it

3. Clone **Figure1 COVID** dataset from this GitHub [link](https://github.com/agchung/Figure1-COVID-chestxray-dataset) into `Original Data` folder 

4. Clone **Actualmed COVID** dataset from this GitHub [link](https://github.com/agchung/Actualmed-COVID-chestxray-dataset) into `Original Data` folder 

5. Download both **Viral Pneumonia** and **Normal X-ray** dataset from this Kaggle [link](https://www.kaggle.com/tawsifurrahman/covid19-radiography-database) and unzip into `Original Data` folder 

6. Download **Kermany et. al** dataset from this Mendeley [link](https://data.mendeley.com/datasets/rscbjbr9sj/2#file-41d542e7-7f91-47f6-9ff2-dd8e5a5a7861) and unzip into `Original Data` folder. Then add their train and test data into their respective folders in the `Data` folder.

<div id="notebooks"></div>

### Notebooks
1. The `networks.ipynb` notebook can be used to run the different networks' trials on:
    * Original Data
    * Not augmented
    * Without Kermany et. al dataset
2. The `vgg_best_network.ipynb` notebook can be used to run the best network vgg on:
    * Entire Data
    * Augmented (In the notebook the code for augmentation should be run once as it creates the augmented data and adds it to `train_augmented` folder)
        * Flippig horizontal
        * Contrast adjustments
    * Kermany et. al dataset. 
3. The `download_data.ipynb` notebook can be used to:
    * split the data into test and train for the datasets that don't have a split
    * read the image files and move them into the test and train folders in `Data` folder.


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- Future Works -->

<div id="future"></div>


## Future Work

- [ ] Use Kermany et. al CT-data
- [ ] Segment the lungs before classification
- [ ] Add heirarichal classification into different types of pneumonia
- [ ] Use class activation maps to see which areas of the lung are most associated with each class
- [ ] Add a COVID-19 class and do multiclass classification


<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->

<div id="contact"></div>

## Contact

* Merna Bibars - merna.bibars@eng.cu.edu.eg

* Peter Emad - peter.emad@eng.cu.edu.eg


Project Link: [https://github.com/Merna-Atef/pneumonia-detection-xray](https://github.com/Merna-Atef/pneumonia-detection-xray)

<p align="right">(<a href="#top">back to top</a>)</p>






[contributors-shield]: https://img.shields.io/github/contributors/Merna-Atef/pneumonia-detection-xray.svg?style=for-the-badge
[contributors-url]: https://github.com/Merna-Atef/pneumonia-detection-xray/graphs/contributors
