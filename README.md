个人临时转化测试
txt文本节点在线转换yaml文件，在openclash上yaml文件下载内核检测过程中报错：level=error msg="yaml: line 8: did not find expected node content" 
这个错误信息表明你的 OpenClash YAML 配置文件在第 8 行存在语法错误，可根本没看出来哪里报错，删除了第8行也没用……
回归测验：
报错的节点是通过这个连接转的：https://v2rayse.com/node-convert #提供订阅到sub在线模板生成yaml文件在内核检查会报错；
后面看到转换页面有个选V2的版本按钮果断选了https://v2.v2rayse.com/node-convert #转换会提醒是mate内容文件，文件传到在线文件通过openwrt搭建的订阅转换服务sub在线模板生成yaml通过的内核检验可以正常运行使用。

小结：
v2-20240912190.txt
1、第1个地址ttps://v2rayse.com/node-convert  #报错  
附：生成yaml文件：v2-20240913160632.yaml
2、第2个v2版本的地址：https://v2.v2rayse.com/node-convert  #正常
附：生成yaml文件：v2rayse_2024-09-13 17_14_36.yaml
