add_executable(ExampleTest test.cpp)

target_link_libraries(ExampleTest gtest gtest_main)

enable_testing()

add_test(NAME MyTests COMMAND ExampleTest)
