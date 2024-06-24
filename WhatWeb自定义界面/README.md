# WhatWeb

# 1. 简介
WhatWeb 识别网站。它的目标是回答这个问题，“那个网站是什么？WhatWeb 认可 Web 技术，包括内容管理系统 （CMS）、博客平台、统计/分析包、JavaScript 库、Web 服务器和嵌入式设备。WhatWeb 有超过 1800 个插件，每个插件都可以识别不同的东西。WhatWeb 还可以识别版本号、电子邮件地址、帐户 ID、Web 框架模块、SQL 错误等。

WhatWeb可以是隐蔽的和快速的，也可以是彻底的但缓慢的。WhatWeb 支持侵略性级别，以控制速度和可靠性之间的权衡。当您在浏览器中访问网站时，该交易包含许多提示，说明哪些 Web 技术正在为该网站提供支持。有时，单个网页访问包含足够的信息来识别网站，但当它没有时，WhatWeb 可以进一步询问该网站。默认的攻击级别称为“隐身”，是最快的，只需要一个网站的一个 HTTP 请求。这适用于扫描公共网站。开发了用于渗透测试的更具侵略性的模式。

大多数 WhatWeb 插件都是彻底的，可以识别从微妙到明显的一系列线索。例如，大多数 WordPress 网站都可以通过元 HTML 标签来识别，例如“”，但少数 WordPress 网站删除了这个识别标签，但这并不能阻止 WhatWeb。WordPress WhatWeb 插件有超过 15 项测试，包括检查网站图标、默认安装文件、登录页面以及检查相对链接中的“/wp-content/”。
- 官网：[https://github.com/urbanadventurer/WhatWeb](https://github.com/urbanadventurer/WhatWeb)
- 官方文档：[https://morningstarsecurity.com/research/whatweb](https://morningstarsecurity.com/research/whatweb)
- 工具版本：0.5.2
- 需要的Ruby环境版本：3.2.2+
- 支持的TangGo版本：v1.4.8+
# 2. 使用方法
- 打开快捷工具，右上角点击导入，找到"WhatWeb自定义界面/WhatWeb-识别网站扫描器.txt"进行导入
  ![import.png](image/import.png)
- 配置工具路径,在"自定义界面"分组找到"WhatWeb-识别网站扫描器"，点击编辑.
- 选择系统内置ruby环境（该工具需要ruby运行，不存在则安装ruby）,ruby初始化安装WhatWeb见官方文档：[https://morningstarsecurity.com/research/whatweb](https://morningstarsecurity.com/research/whatweb)
- 选择WhatWeb实际路径 通过[https://github.com/urbanadventurer/WhatWeb/releases](https://github.com/urbanadventurer/WhatWeb/releases)下载工具
  备注（在ruby安装目录下找到bundle,在WhatWeb实际路径执行: ruby\bin\bundle install）
 ![update.png](image/update.png)
- 打开工具，选择模板，配置参数，启动
  ![switch.png](image/switch.png)
# 3. 运行截图

- 基本扫描
  ![base.png](image/base.png)
- 文件中读取目标并扫描
  ![read.png](image/read.png)
