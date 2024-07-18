file(GLOB_RECURSE FILES
"src/*.cpp" 
"src/*.h"
)
set(TARGET_NAME AngelScriptTest)
add_executable(${TARGET_NAME} ${FILES})
target_include_directories(${TARGET_NAME} PRIVATE src)
target_link_libraries(${TARGET_NAME} PRIVATE angelscript)
target_link_libraries(${TARGET_NAME} PRIVATE angelscript_add_on)