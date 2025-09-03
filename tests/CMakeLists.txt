# SPDX-FileCopyrightText: 2021 Aleix Pol Gonzalez <aleixpol@kde.org>
# SPDX-License-Identifier: BSD-3-Clause

if (NOT LAYER_SHELL_QT_DECLARATIVE)
	message(FATAL_ERROR "The example program cannot be built if LAYER_SHELL_QT_DECLARATIVE=OFF")
endif()

add_executable(layershellqt-test main.cpp)
target_link_libraries(layershellqt-test PRIVATE LayerShellQtInterface Qt::Qml Qt::Gui)
