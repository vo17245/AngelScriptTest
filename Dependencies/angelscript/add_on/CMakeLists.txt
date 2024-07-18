file(GLOB_RECURSE FILES
"./*.cpp" 
"./*.h"
)

set(TARGET_NAME angelscript_add_on)
add_library(${TARGET_NAME} ${FILES})
target_link_libraries(${TARGET_NAME} PUBLIC angelscript)
target_include_directories(${TARGET_NAME} PUBLIC ./)