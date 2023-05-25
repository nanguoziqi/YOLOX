# YOLOX
## 1.项目说明
  本项目为YOLOX模型的训练和测试，本项目在Kaggle网站上运行。
## 2.代码说明
### 2.1Kaggle环境准备
```Python
import numpy as np # linear algebra
import pandas as pd # data processing, CSV file I/O (e.g. pd.read_csv)

# 输入数据文件在只读“../input/“ 目录

import os
for dirname, _, filenames in os.walk('/kaggle/input'):
    for filename in filenames:
        print(os.path.join(dirname, filename))
```
### 2.2下载YOLOX模型
```Python
#函数调用
import warnings
warnings.filterwarnings("ignore")

import ast
import os
import json
import pandas as pd
import torch
import importlib
import cv2 

from shutil import copyfile
from tqdm.notebook import tqdm
tqdm.pandas()
from sklearn.model_selection import GroupKFold
from PIL import Image
from string import Template
from IPython.display import display
```
