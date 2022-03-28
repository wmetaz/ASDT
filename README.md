# ASDT
This is the pytorch version code of ASDT. The code was based RRM <https://github.com/zbf1991/RRM>. Thanks for their nice work!

# Installation
The project needs 1 NVIDIA 1080TI, python=3.6, pytorch=0.4.1.

# Data preparation
You can download the PASCAL VOC 2012 dataset from here <http://host.robots.ox.ac.uk/pascal/VOC/voc2012/>

Please Change your data path in the line 43 in the train_from_cls_weight.py and line 31 in the infer_RRM.py, such as "datasets/VOC2012/VOCdevkit/VOC2012/JPEGImages"

As for the pretrain model, you can refer to RRM.

# Training from a pretrained classification model:
python train_from_cls_weight.py

# Test

python infer_RRM.py

# Evaluation

python cal_miou.py

# Ours model

Ours model was put into the website<>, you can download the model and evaluation.

# Retrain  

When you get the pseudo label on the train dataset, you can use them to train a fully-supervised semantic segmentation model, like Deeplab v1, Deeplab v2, we used the following code, WSSS_mmseg <https://github.com/Eli-YiLi/WSSS_MMSeg>,Deeplab v2<https://github.com/kazuto1011/deeplab-pytorch> thanks for their great work! 
