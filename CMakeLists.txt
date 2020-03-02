cmake_minimum_required(VERSION 3.13)

set(CMAKE_CXX_STANDARD 17)
# Отображать все предупреждения в процессе компиляции.
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall")
# Искать инклуды также и в текущей директории.
set(CMAKE_INCLUDE_CURRENT_DIR ON)

project(addressbook-inclass)

set(SOURCES
    main.cpp
    contact.h
    contact.cpp
)

#find_package(Qt5Core CONFIG REQUIRED)
add_executable(${CMAKE_PROJECT_NAME} ${SOURCES})
#target_link_libraries(test Qt5::Core)
