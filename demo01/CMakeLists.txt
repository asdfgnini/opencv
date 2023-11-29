cmake_minimum_required(VERSION 3.25)
project(demo01)

set(CMAKE_CXX_STANDARD 17)

# 设置库搜索路径
LINK_DIRECTORIES(D:\\opencv4.8\\opencv\\build\\x64\\vc16\\lib)
# 设置库目录搜索路径
include_directories(D:\\opencv4.8\\opencv\\build\\include)

add_executable(demo01 main.cpp)

# 链接第三方库
target_link_libraries(demo01 opencv_world480)

