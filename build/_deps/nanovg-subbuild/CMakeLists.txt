# Distributed under the OSI-approved BSD 3-Clause License.  See accompanying
# file Copyright.txt or https://cmake.org/licensing for details.

cmake_minimum_required(VERSION 3.19.8)

# We name the project and the target for the ExternalProject_Add() call
# to something that will highlight to the user what we are working on if
# something goes wrong and an error message is produced.

project(nanovg-populate NONE)

include(ExternalProject)
ExternalProject_Add(nanovg-populate
                     "UPDATE_DISCONNECTED" "False" "GIT_REPOSITORY" "https://github.com/memononen/nanovg" "GIT_TAG" "077b65e0cf3e22ee4f588783e319b19b0a608065"
                    SOURCE_DIR          "C:/Users/zhuof/OneDrive/ETHz/22FS/CMM_8/Assignments/a0-TonyStone191031/build/_deps/nanovg-src"
                    BINARY_DIR          "C:/Users/zhuof/OneDrive/ETHz/22FS/CMM_8/Assignments/a0-TonyStone191031/build/_deps/nanovg-build"
                    CONFIGURE_COMMAND   ""
                    BUILD_COMMAND       ""
                    INSTALL_COMMAND     ""
                    TEST_COMMAND        ""
                    USES_TERMINAL_DOWNLOAD  YES
                    USES_TERMINAL_UPDATE    YES
)


