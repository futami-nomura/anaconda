## About this repository
### Environment for this repository
This repository's file will be execute on Docker.
So if you would like to use these jupyter notebooks, you need follow below

#### 1. docker image pull

```
$ docker pull continuumio/anaconda3
```

#### 2. packages you'll need install

```
$ docker run -i -t continuumio/anaconda3 /bin/bash
root@XXX:/# python -V
Python 3.6.1 :: Anaconda 4.4.0 (64-bit)
root@XXX:/# pip install keras
root@XXX:/# conda create -n tensorflow
root@XXX:/# pip install keras
root@XXX:/# pip install keras --upgrade
```

#### 3. then open port 8888 with docker

```
$ docker run -i -p 8888:8888 -t continuumio/anaconda3 /bin/bash
```

#### 4. open jupyter notebook in Docker

```
root@XXX:/# jupyter notebook --ip 0.0.0.0 --allow-root
```
