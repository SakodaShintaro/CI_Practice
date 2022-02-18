cmake_minimum_required(VERSION 3.10)
project(CI_Practice)

# 共通する設定
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "-march=native")
set(CMAKE_CXX_FLAGS_RELEASE "-O3 -DNDEBUG")

# ソース
file(GLOB SRCS ./*.cc)

# 実行ファイルの定義
add_executable(a.out ${SRCS})
