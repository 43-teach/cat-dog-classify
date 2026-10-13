# cat-dog-classify
猫狗图像分类项目

## 项目简介
本项目基于PyTorch深度学习框架，实现猫狗二分类图像识别。对比不同卷积神经网络模型，使用迁移学习训练模型，完成图像的特征提取、模型训练、性能评估与测试。

## 环境依赖
- Python >=3.8
- PyTorch
- torchvision
- numpy
- Pillow

## 项目文件说明
- `common.py`：公共工具函数、数据预处理代码
- `step1_alexnet.py`：搭建AlexNet基础网络模型
- `step2_pretrain.py`：迁移学习模型训练
- `step4_compare.py`：多模型对比实验
- `step5_test.py`：模型测试，计算准确率等评价指标

> 说明：数据集图片与训练好的模型权重`best_model.pth`体积较大，不存放在本仓库。
> 使用前请自行准备猫狗图片数据集，修改代码内本地数据集路径。

## 运行步骤
1. 准备猫狗数据集，修改代码中的图片文件夹路径
2. 执行 step1_alexnet.py，构建基础模型
3. 运行 step2_pretrain.py 开始迁移学习训练
4. step4_compare.py 对比多个模型效果
5. step5_test.py 在测试集评估模型精度

## 实验结论
迁移学习相比从零训练的网络收敛更快，准确率更高；轻量模型在保证精度的同时推理速度更快。
猫狗图像分类项目
