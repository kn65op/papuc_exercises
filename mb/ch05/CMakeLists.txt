include_directories(${COMMON_INCLUDES} ${CMAKE_CURRENT_SOURCE_DIR})

# UT
add_executable(mb-05-ut ../common/Common.cpp
                        MB_05_UT.cpp
                        MB_05_02.cpp)
target_link_libraries(mb-05-ut gtest_main)

add_custom_target(ch05-mb-ut-run
  COMMAND mb-05-ut
  COMMENT "Run ch05-mb-ut"
)
