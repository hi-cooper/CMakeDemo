# 目录结构

```
|-- libs                  // 三方库目录
|-- modules               // 三方源码目录
|-- build                 // 编译目录
|-- core-sdk              // 项目库目录
|   |-- src               // 源码
|   |-- libs              // 本项目库文件输出目录
|      |-- include        // 开放的API headers
|   |-- bin               // 本项目可执行文件输出目录
|   |-- CMakeLists.txt    // 子cmake
|-- core-sdk-demo         // 项目示例目录
|   |-- src               // 源码
|   |-- bin               // 本项目可执行文件输出目录
|   |-- CMakeLists.txt    // 子cmake
|-- CMakeLists.txt        // cmake
```

# how to

## ubuntu环境下的编译

```shell
# 编译环境
apt-get install -y build-essential

# 编译
cd build
cmake ..
make
```

将在以下路径创建相关文件

```
|-- core-sdk
|   |-- libs
|      |-- include
|         |-- CoreSdk.h   // 开放API headers
|      |-- libCoreSdk.a   // 静态库
|      |-- libCoreSdk.so  // 动态库
|-- core-sdk-demo
|   |-- bin
|      |-- CoreSdkDemo
```

# 