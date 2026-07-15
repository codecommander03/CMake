add_library(OpMul OBJECT)

target_sources(OpMul
  PRIVATE
    OpMul.cxx

  INTERFACE
    FILE_SET HEADERS
    FILES
      OpMul.h
)

target_include_directories(OpMul PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")
