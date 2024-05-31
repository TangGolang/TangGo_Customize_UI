# kscan

# 1. 简介
Kscan是一款纯go开发的全方位扫描器，具备端口扫描、协议检测、指纹识别，暴力破解等功能。支持协议1200+，协议指纹10000+，应用指纹20000+，暴力破解协议10余种。
- 官网：[https://github.com/shadow1ng/fscan](https://github.com/shadow1ng/fscan)
- 支持的TangGo版本：v1.4.8+
# 2. 使用方法
- 打开快捷工具，右上角点击导入，找到"Kscan自定义界面/Kscan-轻量化全方位扫描器.txt"进行导入
  ![import.png](image/import.png)
- 配置工具路径,在"自定义界面"分组找到"Kscan-扫描器"，点击编辑.
- 选择Kscan实际路径 通过[https://github.com/lcvvvv/kscan/releases](https://github.com/lcvvvv/kscan/releases)下载工具
  ![update.png](image/update.png)
- 打开工具，选择模板，配置参数，启动
  ![switch.png](image/switch.png)
# 3. 运行截图
- 运行需设置  --encoding 字段 windows为gbk  linux和mac为utf-8 不然输出会乱码
- 端口扫描模式
  ![base.png](image/port.png)
- Fofa结果检索（需提前配置环境变量:FOFA_EMAIL(邮箱)、FOFA_KEY(key)）
  ![fofa_serch.png](image/fofa_serch.png)
- 暴力破解
 ![blpj.png](image/blpj.png)