
add_executable(mtest mtest.cpp)

target_link_libraries(mtest gtest_main)

add_test(NAME mtest COMMAND mtest)

find_package(Eigen3)
target_link_libraries(mtest Eigen3::Eigen)