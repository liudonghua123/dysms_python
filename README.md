
# SDK 使用说明
阿里云官方SMS的python SDK，由于[aliyun-openapi-python-sdk](https://github.com/aliyun/aliyun-openapi-python-sdk)中没有包含`aliyunsdkdysmsapi`，为方便pip安装，因此未做任何修改，把[dysms_python.zip](http://ytx-sdk.oss-cn-shanghai.aliyuncs.com/dysms_python.zip?spm=a2c4g.11186623.2.6.s3rSMT&file=dysms_python.zip)作为一个git repository托管。

## 如果使用
可以直接执行 `pip install git+https://github.com/liudonghua123/dysms_python.git`，或者在`requirements.txt` 中添加 `git+https://github.com/liudonghua123/dysms_python.git` 这一行。
**以下内容为原来文档自带的！**

## 概述
该python SDK包含MNS、SMS功能，同时兼容python2.6+、python3.0+

## 文档概述
```
├── aliyunsdkdybaseapi   #原aliyunsdkdybaseapi库
│   └── request
├── aliyunsdkdysmsapi    #原aliyunsdkdysmsapi库
│   ├── __init__.py
│   └── request
├── const.py             #配置key、secret等参数
├── demo_sms_api.py      #通过mns获取队列回执
├── demo_sms_query.py    #短信发送状态查询
├── demo_sms_send.py     #短信发送
├── mns_python_sdk       #原mns_python_sdk
│   ├── bin
│   ├── mns
│   ├── sample 
│   ├── sample.cfg
│   ├── sample.py
│   └── setup.py
└── setup.py
```

## SDK使用

* 注：`如果使用python2，则将文中python替换为python2；如果使用python3，则将文中python替换为python3`

### 短信发送或查询状态
* 安装依赖：在最顶层目录执行：python setup.py install
* 短信发送执行demo程序：python demo_sms_send.py
* 查询状态执行demo程序：python demo_sms_query.py

### 通过mns获取队列回执
* 安装依赖1：在最顶层目录执行：python setup.py install
* 安装依赖2：进入目录mns_python_sdk，执行：python setup.py install
* 最顶层目录执行demo执行：python demo_sms_api.py

