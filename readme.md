# intro

> 书海拾贝

书山有路勤为径, 学海无涯苦作舟


## setup jupyter


```bash
$ PYTHON_CONFIGURE_OPTS="--enable-shared" pyenv install 3.8.5
$ pyenv local 3.8.5

$ mkdir ~/.pip
$ echo "[global]\nindex-url = https://mirrors.aliyun.com/pypi/simple/\n[install]\ntrusted-host=mirrors.aliyun.com\n" >> ~/.pip/pip.conf

$ pip install jupyter
$ pip install jupyter_contrib_nbextensions
$ jupyter contrib nbextension install --user

$ jupyter notebook --ip 0.0.0.0 --no-browser
```