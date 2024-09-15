临时节点转化测试

**问题描述：**

> txt文本节点在线转换yaml文件，在openclash上yaml文件下载内核检测过程中报错：level=error msg="yaml: line 8: did not find expected node content"

> 这个错误信息表明你的 OpenClash YAML 配置文件在第 8 行存在语法错误，可根本没看出来哪里报错，删除了第8行也没用……

**回归测验：**

报错文件是使用https://v2rayse.com/node-convert 转换；当通过openwrt搭建订阅转换服务sub模板生成yaml文件，经过内核检验会报错：level=error msg="yaml: line 8: did not find expected node content"

在https://v2rayse.com/node-convert 界面右上角有个旧版本，可选V2，即这个网址 https://v2.v2rayse.com/node-convert  #转换会提醒是mate内容文件 使用该连接生成的yaml文件内核检验没有问题，可以正常使用。

**小结：**

1. 原始节点文本：v2-20240912190.txt
  
2. 第1个地址 https://v2rayse.com/node-convert #报错 ；
  
  附：生成yaml文件：v2-20240913160632.yaml
  
3. 第2个地址：https://v2.v2rayse.com/node-convert      （v2版本）#正常 
  
  附：生成yaml文件：v2rayse_2024-09-13 17_14_36.yaml
  
**问题后续：**
2024-09-16 06:19:55 level=error msg="yaml: unmarshal errors:\n  line 1: cannot unmarshal !!str `No node...` into config.RawConfig"
2024年9月16日，检查内容报错，一直没找到原因……各种检查格式，版本转换都无效。

**调整办法：**
无意中检查openclash配置进行了如下调整：

覆写设置--DNS设置--
Fallback DNS 代理组 (支持正则匹配)  的选项停用掉
  
