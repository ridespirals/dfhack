project(dfhack-tinythread)
add_library(dfhack-tinythread STATIC EXCLUDE_FROM_ALL tinythread.cpp tinythread.h)
if(UNIX)
    target_link_libraries(dfhack-tinythread pthread)
endif()
ide_folder(dfhack-tinythread "Depends")
