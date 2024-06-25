# Nikto

# 1. 简介
Nikto 是一个开源 （GPL） Web 服务器扫描程序，它对 Web 服务器的多个项目进行全面测试，包括 7,000 多个潜在危险的文件/程序，检查 1250 多个服务器的过时版本，以及 270 多个服务器上的版本特定问题。它还检查服务器配置项，例如是否存在多个索引文件、HTTP 服务器选项，并尝试识别已安装的 Web 服务器和软件。扫描项目和插件经常更新，并且可以自动更新。
- 官网：[https://cirt.net/Nikto2](https://cirt.net/Nikto2) 
- git地址：[https://github.com/sullo/nikto](https://github.com/sullo/nikto)
- 工具版本：V2.1.5+
- windows下perl环境版本：v5.3+
- 支持的TangGo版本：v1.4.8+
# 2. 使用方法
- windows需要下载perl运行环境和工具
  ```
  1.通过地址(https://github.com/sullo/nikto/releases)下载版本
  2.通过官网(https://strawberryperl.com/)安装perl运行环境 v5.38.2
  3.运行生成命令示例："D:\Strawberry\perl\bin\perl.exe"  "E:\nikto\program\nikto.pl" -h 127.0.0.1
  ```
- Linux和Mac 通过apt install nikto 或者 yum install nikto 进行安装即可，详情请查看文档：[https://github.com/sullo/nikto/wiki](https://github.com/sullo/nikto/wiki)  
- 打开快捷工具，右上角点击导入，找到"NiktoWeb自定义界面/Nikto-Web服务器扫描仪.txt"进行导入    
  ![d1.png](image/d1.png) 
  ![d2.png](image/d2.png) 
- 配置工具路径,在"自定义界面"分组找到"Nikto-Web服务器扫描仪"，点击编辑.   
  ![d3.png](image/d3.png)
- 选择Nikto-Web服务器扫描仪实际路径 windows为实际下载路径，Linux和Mac 一般为: /usr/bin/nikto   
  ![d4.png](image/d4.png)
- 打开工具，选择模板，配置参数，启动   
  ![d5.png](image/d5.png)
# 3. 运行截图
- 指定端口扫描测试  
  ![p1.png](image/p1.png)
- SSL模式扫描并指定显示输出  
  ![p2.png](image/p2.png)

