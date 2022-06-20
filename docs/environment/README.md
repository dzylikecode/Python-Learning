# 学习环境

## 系统

- Linux

  wsl2: Ubuntu 20.04

## conda

- miniconda

### install

- Download the latest shell script

  ```bash
  wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
  ```

- Make the miniconda installation script executable

  ```bash
  chmod +x Miniconda3-latest-Linux-x86_64.sh
  ```

- Run miniconda installation script

  ```bash
  ./Miniconda3-latest-Linux-x86_64.sh
  ```

- Make sure the miniconda installation is complete

  ```bash
  conda info
  ```

- deactivate the default environment

  ```bash
  conda config --set auto_activate_base false
  ```

### commands

- [Conda 常用命令整理](https://blog.csdn.net/menc15/article/details/71477949)

- 高频

  `conda create --name your_env_name python=3.5`

  `conda env list`

  `activate your_env_name`

  `deactivate`

  `conda remove --name your_env_name --all`

  `conda create --name new_env_name --clone old_env_name `

- 分享环境

  当前环境

  - 导出: `conda env export > environment.yml`
  - 导入: `conda env create -f environment.yml`
