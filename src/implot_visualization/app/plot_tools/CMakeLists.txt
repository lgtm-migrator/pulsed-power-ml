add_library(
    plot_tools OBJECT
        "plot_tools.cpp"
)

target_include_directories(
    plot_tools BEFORE
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
)

target_link_libraries(
    plot_tools
    PUBLIC
        deserializer
        implot
)