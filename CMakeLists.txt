project(testlib)
cmake_minimum_required(VERSION 3.16)

add_executable(testlib pdftohtml.cc)
target_include_directories(testlib PUBLIC include)

target_link_libraries(testlib ${CMAKE_CURRENT_SOURCE_DIR}/xpdf.lib)
