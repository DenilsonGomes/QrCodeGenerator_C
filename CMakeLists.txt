cmake_minimum_required(VERSION 3.8)
project (qrcode)

set (CMAKE_C_STANDARD 99)

# include_directories(".")
add_library(qrcode_lib qrcodegen.c)


add_executable(qrcode_demo qrcodegen-demo.c)
target_link_libraries(qrcode_demo qrcode_lib)