# Linux
## Debian Core ( sử dụng gói lệnh *.deb và apt hoặc apt-install)
Request: ```sudo apt update && sudo apt full-upgrade && sudo apt install curl wget git```
Bước 1: Download Condamini script
```bash
wget -O /tmp/miniconda.sh https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```
```bash
cd /tmp/ && chmod +x miniconda.sh
```
Bước 2: Installer Condamini
```
./miniconda.sh
```
output: 
```
Output

Welcome to Anaconda3 202x.xx

In order to continue the installation process, please review the license
agreement.
Please, press ENTER to continue
>>>
```
Nhấn Enter đến khi thấy output
```
Output
Do you approve the license terms? [yes|no]
```
Nhập <code>yes</code> rồi nhấn Enter
output
```
Anaconda3 will now be installed into this location:
/home/$USER/anaconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/$USER/anaconda3] >>>
```
Nhấn Enter nếu bạn muốn install Miniconda ở vị trí mặc định.
output
```
Preparing transaction: done
Executing transaction: done
installation finished.
Do you wish the installer to initialize Anaconda3
by running conda init? [yes|no]
[no] >>>
```
Nhập <code>yes</code> rồi nhấn enter.
output
```
...
Thank you for installing Anaconda3!
...
```
```
source ~/.bashrc
```
Đã install xong Conda
Bước 3:
Git ED3D
```bash
cd ~/
```
```bash
git clone -b master --single-branch https://github.com/NVlabs/eg3d.git
```
Bước 4:
Thiết Lập Env Conda cho EG3D
```bash
cd eg3d/eg3d
```
```bash
conda env create -f environment.yml
```
Bước 5:
Active EG3D cho Conda
```bash
conda activate eg3d
```
Bước 6:
Chạy GUI EG3D
```bash
python visualizer.py
```
