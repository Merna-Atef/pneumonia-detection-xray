<div id="top"></div>
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="">
    <img src="images/logo.png" alt="Logo" width="300" height="70">
  </a>

  <h3 align="center">Comparative Analysis of Deep Learning Models for Pneumonia Detection using X-ray Images</h3>
  <p align="center">
    This repo contains part of the work for the final project of Ultrasound Tissue Characterization Post-Grad course. This part of the project entails the detection of pneumonia from X-ray images.
  </p>
</div>

[![Contributors][contributors-shield]][contributors-url]
[![Contributors][contributors-shield-p]][contributors-url-p]


<!-- TABLE OF CONTENTS -->

#### Table of contents
---
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
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>





<div id="about-the-project"></div>

<!-- ABOUT THE PROJECT -->
### About The Project
---
We compare the usage of different well-known models for the binary classification task: **Pneumonia** vs **Healthy/Normal** in x-ray images.


<div id="contribution"></div>

<!-- Contribution -->
#### Contribution
* **Data**
    * Combining **6** different datasets for X-ray images
    * Data augmentation
* **Models**
    * Usage of **7** different deep learning models architectures
    * VGG-16, VGG-19, InceptionV3, InceptionResnetV2, MobilenetV3, Resnet50, EfficientnetB3


<div id="built-with"></div>

<!-- Built-with -->
#### Built-With
* [TensorFlow v2.7.0](https://www.tensorflow.org/install)
* [Python v3.9](https://www.python.org/)
* [Jupyter Lab](https://jupyter.org/)


<p align="right">(<a href="#top">back to top</a>)</p>


<div id="getting-started"></div>


<!-- GETTING STARTED -->
### Getting Started
---
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

#### Prerequisites

* pydicom
  ```sh
  pip install pydicom
  ```

<div id="installation"></div>

#### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#top">back to top</a>)</p>

---

<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish












[contributors-shield]: https://img.shields.io/github/contributors/Merna-Atef/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/Merna-Atef
[contributors-shield-p]: 
https://img.shields.io/github/contributors/Peter-Emad/repo_name.svg?style=for-the-badge
[contributors-url-p]:https://github.com/Peter-Emad/