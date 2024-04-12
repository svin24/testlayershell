# SPDX-FileCopyrightText: 2021 Aleix Pol Gonzalez <aleixpol@kde.org>
# SPDX-License-Identifier: BSD-3-Clause
cmake_minimum_required(VERSION 3.5)

project(testlayershell VERSION 0.1 LANGUAGES CXX)

find_package(Qt6 6.2 REQUIRED COMPONENTS Core Gui Qml Quick)
add_executable(layershellqt-test main.cpp)


target_link_libraries(layershellqt-test PRIVATE 
	LayerShellQtInterface 
	Qt6::Core
	Qt6::Gui
	Qt6::Qml
	Qt6::Quick
)
