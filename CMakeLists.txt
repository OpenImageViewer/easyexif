#Easy exif

option(EASY_EXIF_BUILD_DEMO "build freetype wrapper sample" ON)

 file(GLOB sourceFiles
     "./*.h"
     "./*.cpp"
 )

set(TargetName easyexif)
add_library(${TargetName} ${sourceFiles})

if (EASY_EXIF_BUILD_DEMO)
    add_subdirectory(demo)
endif()