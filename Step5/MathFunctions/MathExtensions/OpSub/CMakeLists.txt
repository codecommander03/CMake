add_library(OpSub OBJECT)

target_sources(OpSub
  PRIVATE
    OpSub.cxx

  INTERFACE
    FILE_SET HEADERS
    FILES
      OpSub.h
)

target_include_directories(OpSub PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")
