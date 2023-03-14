project(imageBasics)

set(CMAKE_CXX_FLAGS "-std=c++11")

add_executable(imageBasics imageBasics.cpp)
# 链接OpenCV库
# message("print:" ${OpenCV_LIBS})
target_link_libraries(imageBasics ${OpenCV_LIBS})

add_executable(undistortImage undistortImage.cpp)
# 链接OpenCV库
target_link_libraries(undistortImage ${OpenCV_LIBS})
