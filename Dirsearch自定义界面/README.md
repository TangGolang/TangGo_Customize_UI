# Dirsearch

# 1. 简介
dirsearch 是一个python开发的目录扫描工具。和御剑之类的工具类似，用于扫描网站的敏感文件和目录从而找到突破口，它通过发送HTTP请求来尝试访问可能存在的路径，从而找到不列在网站目录页面上的隐藏资源。dirsearch可以在Windows上安装使用，也可以在kali直接安装使用。

Dirsearch 的主要特点包括：
- 多线程：Dirsearch 采用多线程方式进行目录扫描，充分利用系统资源提高扫描效率。
- 字典支持：它支持使用自定义字典文件来进行目录爆破，你可以使用自己的字典文件或使用内置的常用字典。（注：字典必须是文本文件）
- 支持多种形式的网页（asp，php）
- 支持HTTP代理
- 启发式检测无效的网页
- 指定扩展名：你可以选择限制扫描的文件扩展名范围，以便更加精确地进行目录扫描。
- 进度追踪：Dirsearch 提供实时进度追踪，你可以看到当前扫描的进度和已发现的目录和文件。
- 结果输出：完成扫描后，Dirsearch 会生成详细的扫描报告（纯文本，JSON），展示已发现的隐藏目录和文件。

- 官网：[https://github.com/maurosoria/dirsearch](https://github.com/maurosoria/dirsearch)
- 工具版本：v0.4.3.post1
- 支持的TangGo版本：v1.4.8+
# 2. 使用方法
- 安装界面：如果您是通过界面资源库进行安装的，免去此步骤。如果是本github下载安装，请下载"Dirsearch自定义界面/Dirsearch-高级Web路径暴力破解器.txt"，在主界面的右上角点击导入按钮将该文件导入，如下图所示：
  ![image](https://github.com/user-attachments/assets/66e198fe-6b2e-487e-9294-263750f15114)
  ![import.png](image/import.png)
- 安装python内置环境，您也可以配置成您自己安装的环境<br>
  ![python.png](image/python1.png)
- 从官网下载dirsearch工具，下载地址：https://github.com/maurosoria/dirsearch/releases
- 下载后解压缩到一个不包含空格和中文字符的目录下
- 配置工具路径，在"信息收集工具"分组找到"Dirsearch-高级Web路径暴力破解器"，点击编辑，修改工具路径为您下载的工具的所在路径：
![image](https://github.com/user-attachments/assets/6ce67db3-9f42-415e-b02f-3db92cac033e) 
- 打开工具，选择模板，配置参数，启动<br>
  ![switch.png](image/switch.png)
# 3. 运行截图
- 单个URL扫描<br>
  ![one_scan.png](image/one_scan.png)
- 递归地扫描指定的子目录<br>
  ![read.png](image/dsub.png)
- 深度递归扫描忽略大小写并包含重定向历史<br>
  ![read.png](image/sdlis.png)
# 4. 如果报如下错误：
“DeprecationWarning: pkg_resources is deprecated as an API”，请在工具目录下的requirements.txt尾部下添加：
setuptools==67.6.1，再界面启动执行工具。如果你熟悉python，也可以手工执行如下操作：
1、先卸载setuptools：pip uninstall setuptools
2、再安装67.6.1版本：pip install setuptools==67.6.1 -i https://pypi.tuna.tsinghua.edu.cn/simple
