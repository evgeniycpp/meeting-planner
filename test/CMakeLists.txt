find_package(gtest CONFIG REQUIRED)

add_executable(base_tests base_tests.cpp)
target_link_libraries(base_tests PRIVATE gtest::gtest_main)

include(GoogleTest)
gtest_discover_tests(base_tests)