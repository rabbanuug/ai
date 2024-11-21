```bash
sudo apt update && sudo apt upgrade -y
sudo apt install build-essential git wget curl python3 python3-pip python3-venv openssh-server -y
sudo systemctl enable ssh
sudo systemctl start ssh
ip a # note it down, i will access from another machine
python3 -m venv ~/ml_env
source ~/ml_env/bin/activate
pip install numpy pandas matplotlib scikit-learn jupyterlab torch torchvision
```

### Set Up Jupyter Notebook
If you want to use JupyterLab:
Install JupyterLab:
```bash
pip install jupyterlab
```
Run JupyterLab:
```bash
jupyter lab --no-browser --ip=0.0.0.0
```
Access it from your host browser using <VM-IP>:8888.
