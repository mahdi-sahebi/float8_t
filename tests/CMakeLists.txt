option(BUILD_TESTS "To compile the tests" OFF)
if (BUILD_TESTS)
    message(STATUS "Building tests...")
    set(sources test_float8.cpp)
    set(test ${PROJECT_NAME}_test)

    add_executable(${test} ${sources})

    target_link_libraries(${PROJECT_NAME}_test m)
    target_link_libraries(${PROJECT_NAME}_test gtest)

    target_link_libraries(${PROJECT_NAME}_test elb_numeric)
endif()
