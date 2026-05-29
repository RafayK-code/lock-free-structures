add_executable(tests
    main.cpp
    lock_free_stack/test_stack.cpp
)

target_include_directories(tests PRIVATE third_party)
target_link_libraries(tests lock_free_stack)