# Welcome to NPPD
### NPPD: An Open Dataset Covering Nuclear Pulse for Pile-up Correction
## Introduction
X-rays spectroscopy is used to investigate the elemental composition and chemical states of materials through an energy spectrum. However, in high input-count-rate scenarios, the pile-up effect occurs, distorting the energy spectrum and affecting measurement accuracy. Currently, deep learning methods have been increasingly applied to pile-up correction. Nevertheless, there is a lack of open datasets for improving and measuring the performance of various algorithms. Therefore, the first open time-series nuclear pulse dataset was constructed using the Allpix Squared simulator, which is a well-recognized simulation framework developed by CERN (European Council for Nuclear Research). The dataset contains time-series nuclear pulse data for over a dozen elements. Detailed and diverse annotations are provided to support various deep-learning models. 

<img src="https://github.com/Congyu-Lin/nuclear-pulse-dataset-for-pileup-correction/blob/main/detector.png" width="400"> 

## Dataset structure
Our dataset incorporates the three types
of data. Specifically, for Type I, the input feature consists of a 64 ns clip of pile-
up signal, including 20 ns before and 44 ns after the pulse peak. The label for
Type II is the energy of the particle corresponding to the pulse peak. For Type
ii, the input feature is a 200 ns segment of pile-up signal, with the label being
the original non-pile-up signal that was used to generate the pile-up data. For
Type III, the input is also a 200 ns segment of pile-up signals, while the label is
a vector of the same length as the input. Each value in the vector represents the
energy of a particle arriving at the corresponding time step, or 0 if no particle
arrived
<img src="https://github.com/Congyu-Lin/nuclear-pulse-dataset-for-pileup-correction/blob/main/label.png" width="400"> 

## Note
Due to the large volume of the dataset, we will be gradually uploading the data over the coming period.
