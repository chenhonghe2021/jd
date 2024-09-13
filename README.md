个人节点临时转化测试

###### 问题描述：

> txt文本节点在线转换yaml文件，在openclash上yaml文件下载内核检测过程中报错：level=error msg="yaml: line 8: did not find expected node content"

> 这个错误信息表明你的 OpenClash YAML 配置文件在第 8 行存在语法错误，可根本没看出来哪里报错，删除了第8行也没用……

###### 回归测验：

报错文件是通过该连接转换：https://v2rayse.com/node-convert ，将生成的yaml文件再到openwrt搭建的订阅转换服务sub在线模板生成yaml文件在内核检验会报错；

后面看到转换页面有个旧版本V2按钮果断选了，即这个网址https://v2.v2rayse.com/node-convert #转换会提醒是mate内容文件，文件传到在线文件通过openwrt搭建的订阅转换服务sub在线模板生成yaml通过的内核检验可以正常运行使用。

##### 小结：

1. 原始节点文本：v2-20240912190.txt
  
2. 第1个地址 ttps://v2rayse.com/node-convert #报错 ；
  
  附：生成yaml文件：v2-20240913160632.yaml
  
3. 第2个地址：https://v2.v2rayse.com/node-convert （v2版本）#正常 。
  
  附：生成yaml文件：v2rayse_2024-09-13 17_14_36.yaml
