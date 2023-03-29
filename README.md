#  Comparing Spectral Classification Models Based on End-to-End Supervised Machine Learning and Self-Supervised Machine Learning 
## Self-Supervised Machine Learning Method based on Relational Reasoning and Contrastive Learning

In this work, we propose SpecRRMoco-Net, which is based on self-supervised relational reasoning and contrastive learning to 1D spectral classification problems.  The results show that SpecRRMoco-Net can effectively reduce the time spend by scientists annotating data manually, therefore offering great potential to automate the classification process.

![alt text](https://github.com/sunyue-xfel/Self-Supv-Relational-Reasoning-Learning-and-Contrastive-Learning-Methods_Spectra-Classification/blob/main/img/RRMocoSpec_NET_20230214.png)
Fig 1. Illustration of the proposed 1D spectra classification framework based on the self-supervised SpecRRMoco-Net, which is a combination of Relational Reasoning Network (SpecRR-Net) and Momentum Contrast Network (SpecMoco-Net). The classification framework consists of two parts, i.e., in the first stage, the encoder f_q is trained on unlabeled data to build useful representations, and in the second stage, a small number of labels are used to perform the downstream spectral classification task. 

Open the project in MyBinder: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/HEAD) or Colab: <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/MOCO_RelationReason_SpectraClassification_main%26Linear20220817_b512_LossCoef.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

See our paper "Self-Supervised Approaches to Spectral Classification: Application of Phase Transitions in X-ray Diffraction Data" (https://doi.org/10.21203/rs.3.rs-2599173/v1) for details.


## End-to-End Supervised Machine Learning Models

This study aims to develop deep learning (DL) classification frameworks for one-dimensional (1D) spectral time series. In this work, we deal with the spectra classification problem from two different perspectives, one is a general two-dimensional (2D) space segmentation problem, and the other is a common 1D time series classification problem. We focused on the two proposed classification models under these two settings, the namely the end-to-end binned Fully Connected Neural Network (FCNN) with the automatically capturing weighting factors model and the convolutional SCT attention model. Under the setting of 1D time series classification, several other end-to-end structures based on FCNN, Convolutional Neural Network (CNN), ResNets, Long Short-Term Memory (LSTM), and Transformer were explored. Finally, we evaluated and compared the performance of these classification models based on the High Energy Density (HED) spectra dataset from multiple perspectives, and further performed the feature importance analysis to explore their interpretability. The results show that all the applied models can achieve 100% classification confidence, but the models applied under the 1D time series classification setting are superior. Among them, Transformer-based methods consume the least training time (0.449 s). Our proposed convolutional Spatial-Channel-Temporal (SCT) attention model uses 1.269 s, but its self-attention mechanism performed across spatial, channel, and temporal dimensions can suppress indistinguishable features better than others, and selectively focus on obvious features with high separability.


For more information see our publication 'Sun, Y., Brockhauser, S. and Hegedűs, P., 2021. Comparing End-to-End Machine Learning Methods for Spectra Classification. Applied Sciences, 11(23), p.11520.'

## Summary

| ***Open the whole project in Mybinder or Colab:*** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Comparing-End-to-End-Machine-Learning-Methods-for-Spectra-Classification/HEAD) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Comparing-End-to-End-Machine-Learning-Methods-for-Spectra-Classification">   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
| --- | --- |
| **1. CNN model:** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/HEAD?labpath=SpectralFingerprint_L2Beamtime-CNN-20230307-2mpool3.ipynb)   <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralFingerprint_L2Beamtime-CNN-20210529.ipynb">  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
| **2. LSTM model:**|  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=SpectralClassification-FNN1D-20230312.ipynb)   <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralClassification-FNN1D-20230312.ipynb">   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
| **3. Transformer model:** |  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=SpectralClassification-TRANSFORMER-20210815-MultLen.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralClassification-TRANSFORMER-20210815-MultLen.ipynb">   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>| 
| **4. ConvSCT Attention model:** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=SpectralClassification-Convolutional%20SCT%20Attention-20230306.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralClassification-Convolutional%20SCT%20Attention-20230306.ipynb">   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>| 
| **5. ConvSC Attention model:** |  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=SpectralClassification-Convolutional%20SC%20Attention-20210530.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralClassification-Convolutional%20SC%20Attention-20210530.ipynb">   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | 
| **6. FNN_1D model:** |  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=SpectralClassification-FNN1D-20230312.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralClassification-FNN1D-20230312.ipynb">   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | 
| **7. BINned_Weighting_1D model:** |  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=SpectralClassification-Binned_FCNN_AutoWeighting-20210513.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/SpectralClassification-Binned_FCNN_AutoWeighting-20210513.ipynb">  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | 
| **8. Self-Supervised Classification model:** |  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/main?labpath=MOCO_RelationReason_SpectraClassification_main%26Linear20220817_b512_LossCoef.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sunyue-xfel/Supervised_and_Self_Supervised_DL_Models_for_SpectraClassification/blob/main/MOCO_RelationReason_SpectraClassification_main%26Linear20220817_b512_LossCoef.ipynb">  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | 

The first seven models correspond to end-to-end supervised ML models and the last model corresponds to a self-supervised classification model.
