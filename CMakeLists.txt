add_library(implot implot_items.cpp implot.cpp)

target_include_directories(implot INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

target_link_libraries(implot PUBLIC imgui)
