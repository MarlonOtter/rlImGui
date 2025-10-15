# external/rlImGui/CMakeLists.txt
add_library(rlImGui STATIC rlImGui.cpp)

target_include_directories(rlImGui PUBLIC
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${imgui_SOURCE_DIR}  # Expose imgui.h to rlImGui
)

target_link_libraries(rlImGui PUBLIC raylib imgui)
