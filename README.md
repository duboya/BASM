

# BASM

The relevant datasets and model codes of this paper are summarized as follows.


## 1. Datasets

To validate the performance of BASM, a takeaway industrial dataset Ele.me and a public spatiotemporal recommendation dataset. The experimental data set statistics are shown in Table I below:


Table I: The basic Statistics of datasets.

|          Datasets          | Total Size | Feature |  Users   |  Items  |  Clicks  | Mean Length of User Behaviors |
| :------------------------: | :--------: | :-----: | :------: | :-----: | :------: | :---------------------------: |
|     Ele.me (Industry)      | 2380427866 |   417   | 81086293 | 547354  | 86735276 |             42.86             |
| Spatiotemporal Public Data | 177114244  |   38    | 14427689 | 7446116 | 3140831  |             41.19             |




### 1.1 Industry Dataset

Ele.me is collected from the industrial recommendation platform. It has more than 80 million users and 2 billion samples. 45-day samples are used for training and the samples of the following day are used for testing.



### 1.2 Spatiotemporal Public Data

The dataset contains a total of more than 170 million pieces of data over 8 days, including 7 days of data for model training and 1 day of data for testing. The dataset can be downloaded from link https://tianchi.aliyun.com/dataset/dataDetail?dataId=131047



## 2. Source Code

Since the model is currently deployed in the Ele.me commercial food delivery system, we will only open source all publicly available comparison models in the paper (including Wide & Deep, DIN, AutoInt), which can be reproduced offline through [DeepCTR](https://github.com/shenweichen/DeepCTR).

The comparison models are shown in the table below:

|         Model         | Paper                                                                                                                                                  |
| :-------------------: |:-------------------------------------------------------------------------------------------------------------------------------------------------------|
|      Wide & Deep      | [DLRS 2016][Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf)                                                        |
| Deep Interest Network | [KDD 2018][Deep Interest Network for Click-Through Rate Prediction](https://arxiv.org/pdf/1706.06978.pdf)                                              |
|        AutoInt        | [CIKM 2019][AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                      |
|          M2M          | [WSDM 2022][Leaving No One Behind: {A} Multi-Scenario Multi-Task Meta Learning Approach for Advertiser Modeling](https://arxiv.org/pdf/2201.06814.pdf) |
|         STAR          | [CIKM 2021][One model to serve all: Star topology adaptive recommender for multi-domain ctr prediction](https://arxiv.org/pdf/2101.11427.pdf)          |
|          APG          | [NeurIPS 2022][APG: Adaptive Parameter Generation Network for Click-Through Rate Prediction](https://arxiv.org/pdf/2203.16218.pdf)                     |

The source code of the comparison models can be seen in the **models folder** of this project.

