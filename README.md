# ISCN
This is the code of the paper [*ISCN:Document-Level Event Causality Identification Bridged by Causal Clues*]

## Overview
![image](./imgs/NECI(updata)_08.png)
ISCN (Iterative Semantic Causal Network) is a novel neural network model designed for Document-Level Event Causality Identification (DECI). It addresses the challenges of long-distance dependencies and complex semantic understanding inherent in DECI tasks. The core idea of ISCN is to leverage Causal Clues as bridges to connect scattered events within a document and construct complete causal chains.

### Get the data
The dataset (ver. 1.0) can be obtained from [Tsinghua Cloud](https://cloud.tsinghua.edu.cn/f/a7d1db6c44ea458bb6f0/?dl=1) or [Google Drive](https://drive.google.com/file/d/1fxomYO6zPl5DDrDr_HeWFK14s8BpW1z-/view?usp=sharing).

You can also download `MAVEN-ERE` and other processed datasets used in our experiments with the scripts in `/data`:
```bash
cd data
bash download_maven.sh
bash download.sh
cd ../
```
## Requirements
python==3.12
- transformers>=4.48.0
- matplotlib==3.5.3
- numpy==1.21.5
- scikit-learn==1.0.2
- scipy==1.7.3
- torch==2.0.1+cu118
- torch_scatter==2.0.9
- torch_geometric==2.1.0.post1
- tqdm==4.64.1
- torch_sparse



For the complete version of the datasets, please visit the [EventStoryLine](https://github.com/tommasoc80/EventStoryLine/).
### Training

Under `src` directory, run the following scripts to start training: 

(1) ESC: 
```
  sh train_ESC.sh
```

(2) MAVEN-ERE: 
```
  sh train_MAVEN.sh
```
