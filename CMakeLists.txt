add_library(rlImGui STATIC rlImGui.cpp)

target_include_directories(rlImGui PUBLIC
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${IMGUI_INCLUDE_DIR}  # Now this resolves correctly
)

target_link_libraries(rlImGui PUBLIC raylib imgui)
