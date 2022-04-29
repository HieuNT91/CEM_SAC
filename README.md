# CEM_SAC
[![MIT licensed](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE.md)

Source code for paper "Combining Soft-Actor Critic with Cross-Entropy Method for Policy Search in Continuous Control". IEEE CEC 2022



Hieu Trung Nguyen, Khang Tran and Ngoc Hoang Luong
<!-- In IEEE CEC 2022. -->
## Setup
- Clone this repo: 
```
$ git clone https://github.com/junhill-2000/eTD3.git
$ cd CEC_SAC
```
- The following packages are needed:
```
tianshou==0.4.4
gym==0.19.0
mujoco_py==2.0.2.13 (need to install mujoco200 from http://www.mujoco.org/ or try my sh script)
```
## Install Old Version of Mujoco
```
gdown --id 1H6PkDQGlp5bUfvanbYPv-Of9ZZ8OSDHJ
chmod +x mujoco_colab.sh 
./mujoco_colab.sh

import os
os.environ['LD_LIBRARY_PATH'] += ':'
os.environ['LD_LIBRARY_PATH'] += '/root/.mujoco/mujoco200/bin'
os.environ.get("LD_LIBRARY_PATH", "")
```

## Usage

### train agent with CEM_SAC
```
python3 cem_sac.py --task [environment_name] --seed [seed] --logdir [log_directory]
```

### Visualize (comming soon)

## Acknowledgement
Our source code is inspired by:
- [CEM-RL by Pourchot et al.](https://github.com/apourchot/CEM-RL)
- [Tianshou library](https://github.com/thu-ml/tianshou/tree/master/examples/mujoco)
