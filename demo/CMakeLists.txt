cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
add_executable (EasyExifDemo "demo.cpp")
target_include_directories(EasyExifDemo PRIVATE ../)
target_link_libraries(EasyExifDemo easyexif)
