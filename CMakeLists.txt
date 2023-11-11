file(GLOB_RECURSE SMF_SOURCES
    "src/*.c"
    "src/*.cpp"
)

set(SMF_INCLUDE_DIRS "./include")


idf_component_register(
    SRCS ${SMF_SOURCES}
    INCLUDE_DIRS ${SMF_INCLUDE_DIRS}
)