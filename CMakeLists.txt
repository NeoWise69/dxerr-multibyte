#####################################################################
##  File: CMakeLists.txt                                           ##
##                                                                 ##
##  Copyright (c) Microsoft Corporation. All rights reserved.      ##
##  Licensed under the MIT License.                                ##
##                                                                 ##
##  Heavily modified by WhiteGear Studio for in-house game engine. ##
##  Re-Licensed under the MIT License.                             ##
##                                                                 ##
##  This version supports both UNICODE and ANSI strings.           ##
#####################################################################

SET(DXErr_SOURCES DXErr_ansi.cpp DXErr_wide.cpp)

IF(WIN32)
    ADD_LIBRARY(DXErr STATIC ${DXErr_SOURCES})
ENDIF()
