# Distributed under the OSI-approved BSD 3-Clause License.  See accompanying
# file Copyright.txt or https://cmake.org/licensing for details.

cmake_minimum_required(VERSION 3.19.8)

# We name the project and the target for the ExternalProject_Add() call
# to something that will highlight to the user what we are working on if
# something goes wrong and an error message is produced.

project(glm-populate NONE)

include(ExternalProject)
ExternalProject_Add(glm-populate
                     "UPDATE_DISCONNECTED" "False" "URL" "https://github.com/g-truc/glm/releases/download/0.9.9.7/glm-0.9.9.7.zip" "URL_HASH" "MD5=da4740b5b41a1e2ccb2955af74e7c298"
                    SOURCE_DIR          "C:/Users/zhuof/OneDrive/ETHz/22FS/CMM_8/Assignments/a0-TonyStone191031/build/_deps/glm-src"
                    BINARY_DIR          "C:/Users/zhuof/OneDrive/ETHz/22FS/CMM_8/Assignments/a0-TonyStone191031/build/_deps/glm-build"
                    CONFIGURE_COMMAND   ""
                    BUILD_COMMAND       ""
                    INSTALL_COMMAND     ""
                    TEST_COMMAND        ""
                    USES_TERMINAL_DOWNLOAD  YES
                    USES_TERMINAL_UPDATE    YES
)


