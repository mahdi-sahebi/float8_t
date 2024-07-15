set(sources test_float8.cpp)
set(test ${PROJECT_NAME}_test)

add_executable(${test} ${sources})

target_link_libraries(${PROJECT_NAME}_test m)
target_link_libraries(${PROJECT_NAME}_test gtest)

target_link_libraries(${PROJECT_NAME}_test elb_numeric)
