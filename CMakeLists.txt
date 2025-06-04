#-------------------------------------------------------------------------------
# Copyright (c) Bob Johnson 2025 - All Rights Reserved
#
# Unauthorized copying of this file, via any medium is strictly prohibited.
# Proprietary and confidential.
#-------------------------------------------------------------------------------

add_library(stb_image STATIC)

set_target_properties(stb_image
	PROPERTIES
		LINKER_LANGUAGE CXX
)

# Source
include(CMakeSources.cmake)

target_sources(stb_image
	PRIVATE 
		${SRC_IMAGE}
)

# Include
target_include_directories(stb_image
PUBLIC  "."
)

#-------------------------------------------------------------------------------

