# qpress - 跨平台高速文件压缩工具（支持 Windows 编译）

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/PierreLvx/qpress/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/PierreLvx/qpress/tree/master)

本仓库基于 [QuickLZ 官方网站](http://www.quicklz.com/) 上最后公开版本的 **qpress**，
并进行了多项补丁修改与改进 —— **已支持在 Windows 系统上成功编译运行**。

✅ 现已在 Windows（MSVC）环境中测试通过。  
---

## 🧩 编译命令
g++ -O3 -o qpress -x c quicklz.c dirent_win.c -x c++ qpress.cpp aio.cpp utilities.cpp -lpthread -Wall
     -Wextra -Werror