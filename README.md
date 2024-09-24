# AI-mammography
[![mammography](https://img.shields.io/badge/uyen-mammogram-blue)](https://github.com/UeenHuynh/AI-mammography.git)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/UeenHuynh/AI-mammography.git)

This is a summary of recent mammography methods. Please feel free to contact me (uyenhuynhkhoiminh.1.1@gmail.com) if I miss some papers. Issues and PRs are also welcomed! 

## Mammography 2D datasets
| Dataset| Published | Dataset| CODE | PDF             |
| :---------| :----------------------: | :-------------------------------------------------------------------------:| :--------------------: |  :--------------- |
|A review of the machine learning datasets in mammography, their adherence to the FAIR principles and the outlook for the future| Nature|NA|[Dataset](NA)|[Paper](https://www.nature.com/articles/s41597-023-02430-6.pdf)|
|The Chinese Mammography Database (CMMD)| Nature|TCIA|[Dataset](https://www.cancerimagingarchive.net/collection/cmmd/)|[Paper](https://www.nature.com/articles/s41597-023-02025-1)|
|Curated Breast Imaging Subset of DDSM (CBIS-DDSM)| Nature|TCIA|[Dataset](https://www.cancerimagingarchive.net/collection/cbis-ddsm/)|[Paper](https://www.nature.com/articles/sdata2017177)|
|Mammographic Image Analysis Society (MIAS) database v1.21| University of Cambridge|TCIA|[Dataset](https://www.repository.cam.ac.uk/bitstreams/5960ab2b-5ea2-4db1-96ac-15b3605e7485/download)|[Paper](https://www.researchgate.net/publication/243788073_Themammographic_image_analysis_society_digital_mammogram_database)|
|INBreast| NA|NA|[Dataset](https://www.kaggle.com/datasets/ramanathansp20/inbreast-dataset)|[Paper](inbreast.pdf)|


## Mammography deep learning detection tools
| Tool| Published | Dataset| CODE | PDF             |
| :---------| :----------------------: | :-------------------------------------------------------------------------:| :--------------------: |  :--------------- |
|Deep Learning to Improve Breast Cancer Detection on Screening Mammography (End-to-end Training for Whole Image Breast Cancer Screening using An All Convolutional Design)| NatureResearch|CBIS-DDSM, INbreast|[Code](https://github.com/lishen/end2end-all-conv)![Github stars](https://img.shields.io/github/stars/lishen/end2end-all-conv)|[Paper](https://www.nature.com/articles/s41598-019-48995-4.pdf)|
|Mammo-CLIP: A Vision Language Foundation Model to Enhance Data Efficiency and Robustness in Mammography| Arxiv|UPMC, RSNA|[Code](https://github.com/batmanlab/Mammo-CLIP)![Github stars](https://img.shields.io/github/stars/batmanlab/Mammo-CLIP)|[Paper](https://arxiv.org/pdf/2405.12255)|
|DIGITAL EYE for MAMMOGRAPHY: Deep Transfer Learning and Model Ensemble based Open-Source Toolkit for Mass Detection and Classification.| Arxiv|NA|[Code](https://github.com/cbddobvyz/digitaleye-mammography)![Github stars](https://img.shields.io/github/stars/cbddobvyz/digitaleye-mammography)|[Paper](https://arxiv.org/pdf/2405.12255)|
|Amazon SageMaker Mammography Classification Workshop| Arxiv|NA|[Code](https://github.com/aws-samples/mammography-classification-workshop)![Github stars](https://img.shields.io/github/stars/aws-samples/mammography-classification-workshop)|-|
|Pixel wise Breast Mammography Image Segmentation using Generative Adversarial Networks| Arxiv|CBIS-DDSM|[Code](https://github.com/ankit-ai/GAN_breast_mammography_segmentation)![Github stars](https://img.shields.io/github/stars/aws-samples/mammography-classification-workshop)|[Paper](https://github.com/ankit-ai/GAN_breast_mammography_segmentation/blob/master/images/Screen%20Shot%202019-01-06%20at%209.47.40%20PM.png?raw=true)|
|OncoNet: Developing Deep Learning Models for Mammography| -|Onco|[Code](https://github.com/yala/OncoNet_Public)![Github stars](https://img.shields.io/github/stars/yala/OncoNet_Public)|-|
|Mirai: Mammography-based model for breast cancer risk| -|Onco|[Code](https://github.com/yala/Mirai)![Github stars](https://img.shields.io/github/stars/yala/Mirai)|-|
|Deep Multi-instance Networks with Sparse Label Assignment for Whole Mammogram Classification| Arxiv|INBreast|[Code](https://github.com/wentaozhu/deep-mil-for-whole-mammogram-classification)![Github stars](https://img.shields.io/github/stars/wentaozhu/deep-mil-for-whole-mammogram-classification)|[Paper](https://arxiv.org/pdf/1705.08550)|


## Mammography visualization & annotation
Common
## Literature review
### SOTA in AI Mammography Detection
| Tool| Published | Dataset| Model | PDF             |
| :---------| :----------------------: | :-------------------------------------------------------------------------:| :--------------------: |  :--------------- |
|Automated abnormalities detection in mammography using deep learning| Springer-2024|INBrest, CBIS-DDSM|CNN, U-Net, AUNet|[Paper](https://link.springer.com/article/10.1007/s40747-024-01532-x)|
|Applying Deep Learning Methods for Mammography Analysis and Breast Cancer Detection| Appl. Sci. 2023|-|CAM|[Paper](https://www.mdpi.com/2076-3417/13/7/4272)|
|Applying Deep Learning Methods for Mammography Analysis and Breast Cancer Detection| Appl. Sci. 2023|INBrest, CBIS-DDSM|CAM|[Paper](https://www.mdpi.com/2076-3417/13/7/4272)|

## Gaps in Current Research
1. Data Scarcity: Models trained on small datasets, may not generalize well across diverse populations. Recent studies have suggested the use of self-supervised learning to mitigate the issue of limited labeled data [Paper](https://www.frontiersin.org/journals/oncology/articles/10.3389/fonc.2024.1281922/full)
2. Generalization and Overfitting: Many AI models, particularly those based on deep learning, suffer from overfitting due to the limited diversity in mammogram datasets. A typical solution involves cross-validation, but without appropriate regularization techniques like dropout, these models might still fail on unseen data​ [Paper](https://link.springer.com/article/10.1007/s40747-024-01532-x)
3. Multi-Modal Integration: AI systems currently focus predominantly on mammograms, but integration with other imaging techniques like MRI or ultrasound has shown promise. Combining data from multiple imaging modalities could improve diagnostic accuracy and tackle the issue of false positives​ [Paper](https://www.mdpi.com/2076-3417/12/9/4616)

## Recommendations for Future Research
1. Hybrid AI Models: Combining classification and segmentation in one model can improve diagnostic outcomes. Multi-task learning networks
2. Explainable and Robust AI: To increase clinical adoption, more research should focus on explainability.
3. Transfer Learning and Domain Adaptation: Applying transfer learning from large datasets (even those outside mammography) could help address the issue of limited medical datasets. Models pretrained on general image datasets could be fine-tuned for mammogram analysis, as recent research has shown promising results in this area