cmake_minimum_required(VERSION 3.14)
project(pnl_calculator)

include(FetchContent)
FetchContent_Declare(
  googletest
  URL https://github.com/google/googletest/archive/refs/tags/release-1.14.0.zip
)
FetchContent_MakeAvailable(googletest)

add_subdirectory(app)
add_subdirectory(tests)
