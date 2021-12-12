<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/AustralianSDAF">
    <img src="imgs/asdaf_logo.png" alt="Logo" width="400">
  </a>

  <h3 align="center">Land Cover Classification Using a Convolutional Neural Network (CNN)</h3>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

Land use describes the use of land surfaces by humans. Land cover describes physical features that occupy the surface of the Earth, such as water, forest, urban structures, vegetation, etc.

We rely on accurate land use data for both scientific and administrative purposes. In particular, land cover and land use data are critical in effective planning to ensure that different structures are positioned on the landscape in a rational manner. For example, land use information can be used to ensure that residential neighborhoods are positioned close to commercial centers and transportation services and distant from industrial areas. Land use data is also an important components of climatic and hydrologic modelling such as estimating the runoff of rainfall from varied surfaces into stream systems.

While it is possible to acquire land use and land cover data through direct observation by visiting each site in person, this process can be costly and time consuming. A more efficient approach is to use satellite imagery and machine learning to automate the process.

In this tutorial, we will develop and evaluate a deep learning model to automatically classify land cover types from satellite imagery. Specifically, we will achieve the following:   

1. Download the EuroSAT dataset for training our model from the TensorFlow Datasets platform
2. Clean and prepare the EuroSAT dataset to feed into a deep ML model
3. Split the cleaned data into training and test sets
4. Define and build a CNN model using the Keras framework
5. Fit the model to our training data
6. Evaluate the accuracy of our model on the test set using visualisation techniques
7. Use the model to make predictions on a new image


<!-- GETTING STARTED -->
## Getting Started

To get started with this tutorial, open and run the `Training - Land Cover Classification using CNNs` notebook and the `Making Predictions - Land Cover Classification` notebook, in that order.

The repository contains three Jupyter notebooks:
1. Training - Land Cover Classification using CNNs – contains the code to download a training dataset and train a model
2. Making Predictions - Land Cover Classification – contains the code to use the trained model to make predictions on a new image
3. Helper Functions - Land Cover Classification – contains some helper functions

### Prerequisites

This notebook is developed on the Google Colaboratory and does not have any dependencies. To open the notebooks, select a notebook to open in Github and then click the `Open in Colab` icon.

However, ensure that you have the following directory structure in your Google Drive. Images to use for inference can be downloaded from here. Please place these images in the `Inference_Data` directory.

```
/content/drive/MyDrive/Colab Notebooks/LandCoverClassification
├── Inference_Data
│   ├── T50HLK_20201222T021339_B01.jp2
│   ├── T50HLK_20201222T021339_B02.jp2
│   ├── T50HLK_20201222T021339_B03.jp2
│   ├── T50HLK_20201222T021339_B04.jp2
│   ├── T50HLK_20201222T021339_B05.jp2
│   ├── T50HLK_20201222T021339_B06.jp2
│   ├── T50HLK_20201222T021339_B07.jp2
│   ├── T50HLK_20201222T021339_B08.jp2
│   ├── T50HLK_20201222T021339_B09.jp2
│   ├── T50HLK_20201222T021339_B10.jp2
│   ├── T50HLK_20201222T021339_B11.jp2
│   ├── T50HLK_20201222T021339_B12.jp2
│   ├── T50HLK_20201222T021339_B8A.jp2
│   └── T50HLK_20201222T021339_TCI.jp2
└── TrainedModel
    └── land_cover_classification_pretrained.h5
```

<!-- CONTRIBUTING -->
## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

<!-- LICENSE -->
## License

Distributed under the MIT License.


<!-- CONTACT -->
## Contact

The Australian Space Data Analysis Facility - [@asdaf_space](https://twitter.com/asdaf_space) or Email: info@asdaf.space
