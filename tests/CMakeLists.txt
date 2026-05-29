add_executable(tests
    main.cpp
    atomic_stack/test_stack.cpp
)

target_include_directories(tests PRIVATE third_party)
target_link_libraries(tests atomic_stack)
