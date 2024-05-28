<p align="center">
    <img src="https://github.com/sariahmghames/NeuroSyM-prediction/blob/main/NeuroSyM-sgan/neurosgan_images/logo.png" width="490" height="144" /> 
</p> 

This repository applies a neuro-symbolic approach for enhancing multivariate time series prediction accuracy with application to context-aware human motion prediction 


If you find this work useful, please cite the following paper:

```
@inproceedings{mghames2023,
  title={A Neuro-Symbolic Approach for Enhanced Human Motion Prediction},
  author={Mghames, Sariah and Castri, Luca and Hanheide, Marc and Bellotto, Nicola},
  booktitle={2023 IEEE International Joint Conference on Neural Networks (IJCNN)},
  pages={1--8},
  year={2023},
  organization={IEEE}
}
```


## Results
The following results applies to zara01 test dataset on sgan framework and its neurosym version. We illustrate one single batch with only 6 pedestrians motion for clarity, though the context is much larger.

<p align="center">
    <img src="https://github.com/sariahmghames/NeuroSyM-prediction/blob/main/NeuroSyM-sgan/neurosgan_images/zara01_gt_8ts_neurosym.gif" width="320" height="240" /> 
</p>

<p align="center">
  <img src="https://github.com/sariahmghames/NeuroSyM-prediction/blob/main/NeuroSyM-sgan/neurosgan_images/zara01_pred_8ts_sgan.gif" width="320" height="240" />
  <img src="https://github.com/sariahmghames/NeuroSyM-prediction/blob/main/NeuroSyM-sgan/neurosgan_images/zara01_pred_8ts_neurosym.gif" width="320" height="240" />
</p>

## Training and Testing
Please refer to the readme.md inside each architecture package

```
We welcome any issue or collaborations. You can reach out @ sariahmghames@gmail.com

```
## References

Deployment: https://github.com/sariahmghames/neuROSym
Causal Analysis for time-series data: https://github.com/lcastri/fpcmci
