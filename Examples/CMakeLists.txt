
set(
    DEMO_EXAMPLE_SOURCE_FILES
    build_example.cpp
)

add_executable(DemoApp ${DEMO_EXAMPLE_SOURCE_FILES})

target_link_libraries(
    DemoApp
    PUBLIC
    WidgetFactory
)
