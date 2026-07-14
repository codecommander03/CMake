add_library(Vendor STATIC)
target_sources(Vendor
  PRIVATE
    lib/Vendor.cxx

  PUBLIC
    FILE_SET HEADERS
    FILES
      include/Vendor.h
)

target_include_directories(Vendor
  PUBLIC
    include
)

target_compile_features(Vendor PRIVATE cxx_std_20)

add_library(VendorLib INTERFACE)
target_compile_definitions(VendorLib INTERFACE TUTORIAL_USE_VENDORLIB)

target_include_directories(VendorLib
  INTERFACE
    include
)

target_link_libraries(VendorLib
  INTERFACE
    Vendor
)