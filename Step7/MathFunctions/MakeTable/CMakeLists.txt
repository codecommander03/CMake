# TODO1: Add a MakeTable executable
add_executable(MakeTable)

# TODO2: Add MakeTable.cxx to the MakeTable executable
target_sources(MakeTable
  PRIVATE
    MakeTable.cxx
)

# TODO3: Add a custom command which invokes MakeTable to generate SqrtTable.h

# TODO4: Add a custom target which depends on SqrtTable.h

# TODO5: Add an INTERFACE library to describe the SqrtTable header

# TODO6: Add the current binary directory (and optionally the SqrtTable.h FILE)
#        to a header file set of the interface library

# TODO7: Use add_dependencies to ensure the custom target always runs before
#        targets that depend on the interface library
