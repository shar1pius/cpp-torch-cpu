cmake_minimum_required(VERSION 3.0 FATAL_ERROR)

project(custom_ops)

find_package(Torch REQUIRED)

find_package(OpenCV REQUIRED)

add_executable(app app.cpp)

target_link_libraries(app "${TORCH_LIBRARIES}" ${OpenCV_LIBS})

set_property(TARGET app PROPERTY CXX_STANDARD 11)
