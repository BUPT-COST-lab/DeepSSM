# DeepSSM
This is a TensorFlow implementation of DeepSSM as described in the following paper: 

Xiaoli Liu, Jianqin Yin, Huaping Liu, Jun Liu. DeepSSM: Deep State-Space Model for 3D Human Motion Prediction[C]. 2024 IEEE International Conference on Robotics and Biomimetics (ROBIO). IEEE, 2024: 1184-1189.

![image](https://github.com/user-attachments/assets/e7f155d2-e77a-4973-9d21-6054a645fed8)

## Setup
Required python libraries: tensorflow (>=1.0) + opencv + numpy.
Tested in ubuntu + GTX 1080Ti with cuda (>=8.0) and cudnn (>=5.0).

## Datasets
Human3.6M, 3DPW.
```
the processed data file will be available at: https://pan.baidu.com/s/1iVsvRC_PUeteY3Oi50teHA （password：123a）
```

## Training
Use the `scripts/h36m/DeepSSM_h36m_long_term.sh` or `scripts/h36m/DeepSSM_h36m_short_term.sh` script to train/test the model on Human3.6M dataset for short-term or long-term predictions by the following commands:
```shell
cd scripts/h36m
sh DeepSSM_h36m_long_term.sh  # for short-term prediction on Human3.6M
sh DeepSSM_h36m_short_term.sh # for long-term predictions on Human3.6M
```
You might want to change folders in `scripts` to train on 3DPW dataset.


## Citation
If you use this code for your research, please consider citing:
```latex
@inproceedings{liu2024deepssm,
  title={Deepssm: Deep state-space model for 3d human motion prediction},
  author={Liu, Xiaoli and Yin, Jianqin and Liu, Huaping and Liu, Jun},
  booktitle={2024 IEEE International Conference on Robotics and Biomimetics (ROBIO)},
  pages={1184--1189},
  year={2024},
  organization={IEEE}
}
```

## Contact
A part of code adopts from PredCNN at https://github.com/xzr12/PredCNN.git. 

