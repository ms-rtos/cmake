

# MS-RTOS CMAKE �����������ļ�

������ APP ��Ӧ�þ�̬�⣬ʾ��:


```
cd src/jerryscript
mkdir build
cd build
cmake -G "Unix Makefiles" -DCMAKE_BUILD_TYPE=Release -DJERRY_GLOBAL_HEAP_SIZE=128 -DENABLE_LTO=OFF -DCMAKE_TOOLCHAIN_FILE:PATH="./cmake/toolchain_msrtos.cmake" ..
make
make -j8            // ���̱߳��
make VERBOSE=1 -j8  // �鿴���������ϸ�����Ϣ
```