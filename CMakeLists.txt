cmake_minimum_required(VERSION 3.21)
project(Project5)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "Project5")

find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(Project5 main.cpp UI/mainwindow.cpp UI/mainwindow.h UI/mainwindow.ui global.h Class/userAccount.cpp Class/userAccount.h Class/fileProcess.cpp Class/fileProcess.h tools.cpp UI/depositwindow.cpp UI/depositwindow.h UI/depositwindow.ui UI/userwindow.cpp UI/userwindow.h UI/userwindow.ui)
target_link_libraries(Project5
        Qt::Core
        Qt::Gui
        Qt::Widgets
        )

