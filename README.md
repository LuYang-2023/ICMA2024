<div align="left">

# <div align="center">IDD-YOLOv5: A Lightweight Insulator Defect Real-time Detection Algorithm</div>
**Dear reviewers: The source code and pre-trained model weights will be available upon the acceptance of the paper. Feel free to raise your questions or difficulties in the implementation.

Paper submission number TIM-23-08169R1 was submitted to ieee transactions on instrumentation and measurement.
## <div align="left">Quick Start Examples</div>

<details open>
<summary>Install</summary>

First, clone the project and configure the environment.
[**Python>=3.7.0**](https://www.python.org/), [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).

```bash
git clone https://github.com/LuYang-2023/ICMA2024.git  # clone
cd ICMA2024
pip install -r requirements.txt  # install
```
</details>

<details open>
<summary>Train</summary>

The project uses yolov5s.pt as the pre-trained model, make sure to get it before you start training. 
The dataset WI we used is placed in /root/datasets directory, so make sure the dataset directory is correct during training. 
Then start the training with the following command:

```python
python train.py --weights yolov5s.pt --cfg models/BS-yolov5s.yaml --data data/mydata.yaml
```
</details>


<details>
<summary>Test</summary>

We have provided the trained weights file described in the paper, best.pt. After setting up the deep 
learning environment and preparing the WI dataset, the results can be reproduced using the following command:

```bash
python val.py --data data/mydata.yaml --weights best.pt --task test
```
</details>

## <div align="left"> Weather-Insulator </div>
The WI dataset can be obtained at (https://pan.baidu.com/s/1lgG6BX1Ac9b8_gAwSMOQ0g) with (j8cx).
