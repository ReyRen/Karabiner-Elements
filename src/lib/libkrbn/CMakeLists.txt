cmake_minimum_required (VERSION 3.9)

include (../../common.cmake)

project (krbn)

include_directories(
  ./include
)

add_library(
  krbn
  src/libkrbn.cpp
  src/libkrbn_complex_modifications_assets_manager.cpp
  src/libkrbn_configuration.cpp
  src/libkrbn_connected_devices.cpp
  src/libkrbn_file_monitor.cpp
  src/libkrbn_hid_value_observer.cpp
  src/libkrbn_log_monitor.cpp
  src/libkrbn_system_preferences_monitor.cpp
  src/libkrbn_version_monitor.cpp
  ../../share/frontmost_application_observer_objc.m
)
