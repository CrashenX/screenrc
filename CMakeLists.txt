cmake_minimum_required (VERSION 2.8)
cmake_policy (SET CMP0015 OLD)

set (CMAKE_BUILD_TYPE "" CACHE STRING "")

project (SCREENRC)
set (SCREENRC_VERSION_MAJOR 1)
set (SCREENRC_VERSION_MINOR 0)

set (SCREENRC_INSTALL_DIR "/etc/")

# Copy files with 644 permissions
install(FILES screenrc.custom
    DESTINATION ${SCREENRC_INSTALL_DIR})

