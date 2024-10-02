
set(
    SOURCE_FILES
    Source/WidgetFactory.cpp
)

add_library(
    WidgetFactory
    STATIC
    ${SOURCE_FILES}
)

target_include_directories(
    WidgetFactory
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/Include
)

target_link_libraries(
    WidgetFactory
    PUBLIC
    sfml-graphics
    sfml-audio
    sfml-system
    sfml-window
)
