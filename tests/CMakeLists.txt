#creating executable
add_executable(deriv_test derivatives_test.cpp)
target_link_libraries(deriv_test PRIVATE math_tool_der_int  gtest_main)

include(GoogleTest)
gtest_discover_tests(deriv_test)