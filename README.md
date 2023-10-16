# Track Recommendation for Spotify Playlists using Graph Neural Networks

## Instructions for running the  baseline and our model on the sampled dataset

## Table of Contents

- [Environment](#environment)
- [Dependencies](#dependencies)
- [Dataset](#dataset)
- [Baseline](#baseline)
- [Our Approach](#our-approach)
- [Authors](#authors)

## Environment
It is essential that we setup the virtual environment with the right python version. 

- conda create --name=wstm python=3.7
- conda activate wstm


Use the same kernel to run all cells of the jupyter notebook

It is not recommended to run the code on Google Colab as the Python version creates dependency issues due to StellarGraph imports.

## Dependencies

* python == 3.7
* StellarGraph == 1.2.1
* Chardet
* NLTK
* Pandas
* Numpy
* Tensorflow
* Keras
* SKLearn


## Dataset

- We used the [Spotify Millions Playlist](http://www.recsyschallenge.com/2018/) and sampled 1000 random playlists to generate our own slice of data to be used as our dataset, linked [here](https://gtvault-my.sharepoint.com/:u:/g/personal/rgrover30_gatech_edu/Ed_QWSBuSOhAnFSmxyKhmBkBOPXYDsx02ix3SUKKcMxMiA?e=ThKRmm). 


## Baseline

- We follow the source code of the Automatic Playlist Continuation project from the [Github](https://github.com/TimovNiedek/recsys-random-walk) repository as our baseline.

## Our Approach

- Follow the steps in [environment](#environment) to set up the virtual environment.

- Download the [data](https://gtvault-my.sharepoint.com/:u:/g/personal/rgrover30_gatech_edu/Ed_QWSBuSOhAnFSmxyKhmBkBOPXYDsx02ix3SUKKcMxMiA?e=LtfHbk) and upload it to the working virtual [environment](#environment)

- Run the notebook, which will automatically install the [dependencies](#dependencies) to yield the output.

- We used the PACE cluster with 2 GPU units to run our code with multiprocessing on. If you do not have multiprocessing enabled or GPU's configured, under the "Model Training" subsection please switch the 'use_multiprocessing' variable to "False". 

- With multiprocessing switched on the code should take upto 5-10 minutes to run. Without multiprocessing the code may take more than a few hours, so we recommend utilizing multiprocessing.  

- The metrics for the final output are mentioned in the Evaluation Metrics tab. 

## Authors

- Rynaa Grover
- Reshma Anugundanahalli Ramachandra
- Megha Sharma
- Aryan Vats