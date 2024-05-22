# Neurips2024_MoL2

## 1. Paper Description

### Paper Title : 
A Single-Lead ECG based Lightweight Sleep Apnea Classifier using Signal Image Encoding Algorithms
### Paper Abstract : 
Sleep apnea syndrome constitutes a significant symptom with potential societal impact, experiencing a sharp rise due to factors like the aging population and increasing obesity rates.Polysomnography (PSG) remains the gold standard for diagnosing sleep apnea, yet it poses drawbacks in terms of requiring patients to sleep in a controlled environment, wearing multiple specialized devices, and significant time and cost investments. For the purpose of replacing PSG, much work has focused on developing a model based on single-lead electrocardiogram (ECG) data. However, feature extraction preceding building the model is challenging as it is time-consuming, and the chosen features may greatly affect its performance. To eliminate the cumbersome feature extraction burden, this paper takes a fundamentally different approach to converting given ECG to corresponding image data and then developing a lightweight model using the image data, presenting a methodology applicable to real-world problem-solving scenarios. More specifically, we conduct four sequential experiments to design a sleep apnea classifier using the model. As a result, Our model is expected to contribute to enhancing accessibility by enabling individuals to perform preliminary self-assessment for sleep apnea before seeking diagnosis from healthcare professionals, leveraging mobile devices or edge devices.

## 2. Data
PhysioNet Apnea-ECG Database : <https://physionet.org/content/apnea-ecg/1.0.0/>

## 3. Experiments Settings
| CPU | Intel Xeon Silver 4215R CPU @3.20GHz |
| GPU | NVIDIA RTX A6000 |
| Server | Ubuntu 20.04.6 LTS |
| Environment | Python 3.7.16, PyTorch 1.12.9 |

## 4. Code Description
* base_data Folder : It contains the raw ECG signal data.
* filter Folder : This folder contains the code that processes the original ECG signal using filter and the code that we visualized in the time and frequency domain using the order of filter in this paper.
* MTF_encoding Folder : This folder contains code that divides ECG signals into 1-minute increments and converts them into image data using the MTF algorithm.
* Model_train&test Folder : This folder contains code to train and test the model based on transfer learning.
####* Each code is set up to allow the user to modify as desired, and contains the structure of the MoL2 model designed in this paper.
