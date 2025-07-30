enable_testing()
include(GoogleTest)

add_executable(runTests unittests.cpp)
target_link_libraries(runTests GTest::gtest_main)

gtest_discover_tests(runTests)
