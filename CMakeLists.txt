add_library(implot implot_items.cpp implot.cpp)

target_include_directories(implot INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

# this is heuristically generated, and may not be correct
find_package(imgui CONFIG REQUIRED)
target_link_libraries(implot PRIVATE imgui::imgui)
