# Video-Anomaly


## Real-world Anomaly Detection in Surveillance Videos
### UCF-Crime
UCF-Crime数据集成为了Video-Anomaly任务的一个标志性数据集 `downloading`  
### MIL
一个bag中包含多个样本  
这个bag的label为正：这个bag包含至少一个正样本  
这个bag的label为负：这个bag必须全都是负样本  
基于深度MIL排序，学习bag的异常得分  
代码应用[blog](https://blog.csdn.net/jiafeier_555/article/details/84751928)

## awesome-video-anomaly-detection
主页推的兴趣相关[project](https://github.com/fjchange/awesome-video-anomaly-detection)，新编辑的，列举了Video Anomaly相关算法  

### Future Frame Prediction for Anomaly Detection -- A New Baseline, CVPR 2018  
周报里有体现，[code](https://github.com/StevenLiuWen/ano_pred_cvpr2018)环境已经搭建完成  
dataset: ShanghaiTech `downloading`   https://arxiv.org/pdf/1612.01925.pdf
weights: onedrive `downloading`    
另一个pytorch实现的版本[code](https://github.com/feiyuhuahuo/Anomaly_Prediction)，有diff map图，可以通过diff map去定位与预测偏差值较大的区域，从而实现abnormal location。  Flownet2.0[paper](https://arxiv.org/pdf/1612.01925.pdf)视觉效果不错，Future里用的是flownet2sd和flownet-lite

### Graph Convolutional Label Noise Cleaner:Train a Plug-and-play Action Classifier for Anomaly Detection, CVPR 2019
在UCF-Crime和ShanghaiTech上的TOP2 AUC  avenue
GCN大势所趋，结合Weakly Supervised，GCN-based Video-Anomaly detection应该很有搞头[code](https://github.com/jx-zhong-for-academic-purpose/GCN-Anomaly-Detection)  
[blog](https://www.cnblogs.com/LeeGoHigh/p/11221587.html)和代码有待进一步研究  

### Exploring Background-bias for Anomaly Detection in Surveillance Videos, ACM MM 19  
UCF-Crime上的TOP1 AUC，没有code，Weakly Supervised，[paper](https://sci-hub.pl/10.1145/3343031.3350998)可以研究一下  

---
# Action Recognition  
[mmaction2](https://github.com/open-mmlab/mmaction2) 也是刚刚才release的，对于Kinetics和UCF101的label还是work的  
车上或者其他近景场景下都可以使用，当然需要重新训练
