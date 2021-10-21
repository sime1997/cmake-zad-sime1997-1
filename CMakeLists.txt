cmake_minimum_required(VERSION 3.14)
project(cmake-zad-sime1997 CXX)
enable_testing()
add_subdirectory(test)
add_subdirectory(src)

include(FetchContent)
FetchContent_Declare(
  googletest
  GIT_REPOSITORY https://github.com/google/googletest.git
  GIT_TAG     e2239ee6043f73722e7aa812a459f54a28552929  # release-1.11.0
)
# For Windows: Prevent overriding the parent project's compiler/linker settings
set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
FetchContent_MakeAvailable(googletest)
##################################