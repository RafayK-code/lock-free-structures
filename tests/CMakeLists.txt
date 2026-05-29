add_executable(tests
    main.cpp
    test_stack.cpp
)

target_include_directories(tests PRIVATE third_party)
target_link_libraries(tests lock_free)
