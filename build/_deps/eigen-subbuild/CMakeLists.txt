# Distributed under the OSI-approved BSD 3-Clause License.  See accompanying
# file Copyright.txt or https://cmake.org/licensing for details.

cmake_minimum_required(VERSION 3.19.8)

# We name the project and the target for the ExternalProject_Add() call
# to something that will highlight to the user what we are working on if
# something goes wrong and an error message is produced.

project(eigen-populate NONE)

include(ExternalProject)
ExternalProject_Add(eigen-populate
                     "UPDATE_DISCONNECTED" "False" "URL" "https://gitlab.com/libeigen/eigen/-/archive/3.3.7/eigen-3.3.7.zip" "URL_HASH" "MD5=888aab45512cc0c734b3e8f60280daba"
                    SOURCE_DIR          "C:/Users/zhuof/OneDrive/ETHz/22FS/CMM_8/Assignments/a0-TonyStone191031/build/_deps/eigen-src"
                    BINARY_DIR          "C:/Users/zhuof/OneDrive/ETHz/22FS/CMM_8/Assignments/a0-TonyStone191031/build/_deps/eigen-build"
                    CONFIGURE_COMMAND   ""
                    BUILD_COMMAND       ""
                    INSTALL_COMMAND     ""
                    TEST_COMMAND        ""
                    USES_TERMINAL_DOWNLOAD  YES
                    USES_TERMINAL_UPDATE    YES
)


