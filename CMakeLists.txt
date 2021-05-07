cmake_minimum_required(VERSION 3.10)

project(lottieviewer)

aux_source_directory(./src SRC_FILES)

file(GLOB_RECURSE viewer_SRC
				  "main.cpp"
				  "lottieviewer.cpp")

add_executable(${PROJECT_NAME}  ${SRC_FILES}  ${viewer_SRC})