#-------------------------------------------------------------------------------
# Copyright (c) Bob Johnson 2025 - All Rights Reserved
#
# Unauthorized copying of this file, via any medium is strictly prohibited.
# Proprietary and confidential.
#-------------------------------------------------------------------------------

include(CMakeSources.cmake)

# stb_image
add_library(stb_image STATIC)
set_target_properties(stb_image PROPERTIES LINKER_LANGUAGE CXX)
target_sources(stb_image PRIVATE ${SRC_IMAGE})
target_include_directories(stb_image PUBLIC ".")

# stb_truetype
add_library(stb_truetype STATIC)
set_target_properties(stb_truetype PROPERTIES LINKER_LANGUAGE CXX)
target_sources(stb_truetype PRIVATE ${SRC_TRUETYPE})
target_include_directories(stb_truetype PUBLIC ".")

#-------------------------------------------------------------------------------

