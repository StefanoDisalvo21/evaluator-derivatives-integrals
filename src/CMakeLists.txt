#creating library composed of various file
add_library(math_tool_der_int 
    derivatives.cpp
    helpers_function.cpp
)

#including headers
target_include_directories(math_tool_der_int PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

#adding executable
add_executable(math_evaluator main.cpp)
target_link_libraries(math_evaluator PRIVATE math_tool_der_int)