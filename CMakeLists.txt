# CMakeLists.txt adapted to allow build within ESP-IDF framework

file(GLOB_RECURSE SOURCES ./Fusion/*.c )

set(INCLUDE_DIRS ./Fusion)

idf_component_register(SRCS ${SOURCES}
                       INCLUDE_DIRS ${INCLUDE_DIRS})
