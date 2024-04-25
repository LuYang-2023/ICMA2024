<div align="left">

# <div align="center">IDD-YOLOv5: A Lightweight Insulator Defect Real-time Detection Algorithm</div>
**Dear reviewers: The source code and pre-trained model weights will be available upon the acceptance of the paper. Feel free to raise your questions or difficulties in the implementation.**

Paper ID 433641 has been submitted to IEEE ICMA 2024.
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



```python
python train.py --cfg models/IDD-yolov5.yaml --data data/mydata.yaml
```
</details>


<details>
<summary>Test</summary>


```bash
python val.py --data data/mydata.yaml --weights best.pt --task test
```
</details>

## <div align="left"> The dataset we built </div>
The dataset will be published after acceptance of the paper.
