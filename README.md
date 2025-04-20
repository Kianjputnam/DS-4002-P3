# DS4002 Project 3

#### Kian Putnam, Tenzin Nargee, Vishal Kamalakrishnan 

## Goal

Emergency vehicles such as ambulances, fire trucks, and police cars require swift movement through traffic to respond to critical situations. However, increasing traffic congestion often prevents these vehicles from reaching their destinations in time, potentially putting lives at risk [^fn1]. Our project seeks to accurately classify emergency from non-emergency vehicles utilizing ResNet [^fn2] and the insights from this research could be integrated into intelligent transportation systems.

This dataset was obtained from the Analytics Vidhya JantaHack Computer Vision Hackathon, which originally served as a competition for creating the best model to classifiy emergency vehicles[^fn3]. It includes images of emergency vehicles as well as a training and a test dataset. An account is required to sign up for the Hackathon and collect the data and so we have provided the data as a `.zip` file in the `data` folder.

## Software / Platform

We are using Jupter Notebooks for this program that run on Python 3 (prefferably 3.10+). Our code can be run on **Google Colab** by importing our notebooks. The following files require access to a GPU (or else will be very slow):

1. DataDescription.ipynb

For this file, a **Windows** or **Linux** environment is needed with `pytorch` ..., packages and access to a Nvidia GPU and respective drivers. Additonal packages will be included in the files themselves as a runtime dependency. These files can alternatively be run on **Google Colab** or **Rivanna**. 

All additional files will need a Python environment with the packages `Pandas`, `Numpy`, `Matplotlib`, and with support for `Jupyter Notebooks` and can be run on **Windows**, **Linux**, or **Mac**

## Steps To Reproduce

To reproduce the results of the project first clone the repository the following command in your terminal 
```
git clone https://github.com/Kianjputnam/DS-4402-P3.git
```

You can run the individual files locally (provided you follow the specifications listed in - [Software / Platform](##Software%20/%20Platform)) or can run them in **Rivanna** or **Google Colab**. The image data is provided as a `.zip` file and will have to be unzipped in order to be processed by the notebooks. This can be done using a file archiver such as `7zip` or `winrar`. In **Rivanna** or any other Linux environment, these commands can be run to unzip the file:

```
sudo apt-get install unzip

unzip data.zip
```

The scripts can be run in the order shown by their filenames. While this is not a strict requirements, note that some files need to be run before others in the order shown below

1. DataDescription.ipynb
2. RESNET_Model (2).ipynb

After running the first file, you will have to go through the test data and create a new column, emergency_or_not. This data can be lined up to the images seen in the first file. After labeling the test data, it becomes new_labeled_test.csv. This new file along with the training data in data.zip will be ran through file 2.

### References

[^fn1]: C. Fernandes, "Emergency vs Non-Emergency Vehicle Classification," Analytics Vidhya, Jun. 29, 2020. [Online]. Available: https://medium.com/analytics-vidhya/emergency-vs-non-emergency-vehicle-classification-cc5907977fe5
[^fn2]: "ResNet Model Documentation," Hugging Face. Available: https://huggingface.co/docs/transformers/en/model_doc/resnet
[^fn3]: Analytics Vidhya, "JanataHack: Computer Vision Hackathon," Analytics Vidhya, [Online]. Available: https://www.analyticsvidhya.com/datahack/contest/janatahack-computer-vision-hackathon/#ProblemStatement. [Accessed: 07-Apr-2025].

