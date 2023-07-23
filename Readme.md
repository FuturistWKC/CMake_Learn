[参考文档](https://subingwen.cn/cmake/CMake-primer/)
[参考视频](https://www.bilibili.com/video/BV14s4y1g7Zj?p=1&vd_source=e41e557c965196efc71b2d5de8ad6f36)

### cpp编译
`g++ *.cpp -o app`  
compile files  
`./app`  
run app  

### set的三种作用
1. 定义变量
2. 指定c++标准
3. 指定输出路径
   
`set(EXECUTABLE_OUTPUT_PATH ./app)`./路径为make的路径

### find_package
find_package查找的其实是.cmake文件，文件中包含了编译所需的路径信息

需要使用cmake的方式安装库
find_package(库名称 REQUIRED)
```
库名称_DIR//库所在路径
库名称_INCLUDE_DIRS//库头文件所在路径
库名称_LIBS//链接库路径
```
执行find_package后CMake会设置以上相关个变量
[参考链接1](https://chunleili.github.io/cmake/find_package)
[参考链接2](https://blog.csdn.net/zhanghm1995/article/details/105466372)
[参考视频](https://www.bilibili.com/video/BV18P411K7D1/?spm_id_from=333.337.search-card.all.click&vd_source=e41e557c965196efc71b2d5de8ad6f36)
