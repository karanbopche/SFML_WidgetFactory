enable_testing()

set(
    TEST_SOURCE
    test_sanity.cpp
)

add_executable(
    UNIT_TESTS
    ${TEST_SOURCE}
)

target_link_libraries(
    UNIT_TESTS
    GTest::gtest_main
    GTest::gmock_main
    WidgetFactory
)

target_include_directories(
    UNIT_TESTS
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)

include(GoogleTest)
gtest_discover_tests(UNIT_TESTS)
