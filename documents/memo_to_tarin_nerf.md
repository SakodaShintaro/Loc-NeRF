## Environment
nvidia-smi
Driver Version: 530.30.02

and see docker/env_for_train-nerf/READEME.md

## Commands to exec demo of nerf-pytorch in container
```bash
apt install sudo -y
sudo apt install -y wget unzip
sudo apt install -y python3-pip
sudo apt install -y libgl1-mesa-dev
sudo apt install -y libglib2.0-0
git clone https://github.com/yenchenlin/nerf-pytorch.git
cd nerf-pytorch
pip3 install -r requirements.txt
pip3 install torch==1.13.1
bash download_example_data.sh
python3 run_nerf.py --config configs/lego.txt
```
