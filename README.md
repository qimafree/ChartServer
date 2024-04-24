# ChartServer
基于muduo网络库实现可以工作在nginx、tcp负载均衡环境中的集群聊天服务器和客户端源码

1.文件介绍：
- bin/: 包含编译后的可执行文件，可以直接运行这些程序来启动您的应用或服务。

- build/: 存放编译过程中生成的中间文件，这些文件用于构建最终的可执行文件。

- include/: 通常用于存放头文件（.h 或 .hpp），这些文件包含了函数和类的声明。

- src/: 这个目录包含实际的源代码文件，这些文件将被编译成可执行文件。

- thirdparty/: 包含项目依赖的第三方库文件，这些依赖项是项目运行所必需的。


2.环境配置要求：

为了编译和运行ChatServer，您需要预先配置以下环境：

- JSON 库：ChatServer 使用 JSON 库来处理 JSON 格式的数据交换。
- cmake：ChatServer 使用 CMake 来简化构建过程。请确保您已经安装了 CMake（推荐使用最新版本）
- muduo网络库：muduo 是 ChatServer 的基础依赖，它提供了高性能的网络编程框架。
- MySQL：请确保您的 MySQL 服务正在运行。
- Nginx：作为负载均衡器，需要配置适当的负载均衡策略以优化性能。
- Redis：确保 Redis 服务能正常运行，本项目使用Redis作为中间件消息队列。

3.编译方式：
cd build
re -rf *
cmake ..
make
