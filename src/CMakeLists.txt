


add_executable(main main.cpp)

find_package(Eigen3)
target_link_libraries(main Eigen3::Eigen)

find_package(OpenMP)
target_link_libraries(main OpenMP::OpenMP_CXX)
