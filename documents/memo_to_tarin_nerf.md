## Environment
nvidia-smi
Driver Version: 530.30.02

and see docker/env_for_train-nerf/READEME.md

## Commands to exec demo of nerf-pytorch in container
```bash
apt install sudo -y
sudo apt install -y wget unzip python3-pip libgl1-mesa-dev libglib2.0-0
git clone https://github.com/SakodaShintaro/nerf-pytorch
cd nerf-pytorch
pip3 install -r requirements.txt
bash download_example_data.sh
python3 run_nerf.py --config configs/lego.txt
```
