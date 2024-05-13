## 该项目主要参考以下仓库
* https://github.com/leoxiaobin/deep-high-resolution-net.pytorch
* https://github.com/stefanopini/simple-HRNet

## 文件结构：
```
  ├── model: 搭建网络相关代码
  ├── train_utils: 训练验证相关模块（包括coco验证相关）
  ├── my_dataset_coco.py: 自定义dataset用于读取COCO2017数据集
  ├── person_keypoints.json: COCO数据集中人体关键点相关信息
  ├── train.py: 单GPU/CPU训练脚本
  ├── train_multi_GPU.py: 针对使用多GPU的用户使用
  ├── predict.py: 简易的预测脚本，使用训练好的权重进行预测
  ├── validation.py: 利用训练好的权重验证/测试数据的COCO指标，并生成record_mAP.txt文件
  └── transforms.py: 数据增强相关
```

代码将会逐步优化更新。
