

# MS-RTOS CMAKE 工具链描述文件

适用于 APP 和应用静态库，示例:


```
cd src/jerryscript
mkdir build
cd build
cmake -G "Unix Makefiles" -DCMAKE_BUILD_TYPE=Release -DJERRY_GLOBAL_HEAP_SIZE=128 -DENABLE_LTO=OFF -DCMAKE_TOOLCHAIN_FILE:PATH="./cmake/toolchain_msrtos.cmake" ..
make
make -j8            // 多线程编程
make VERBOSE=1 -j8  // 查看编译过程详细输出信息
```