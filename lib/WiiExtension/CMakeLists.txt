add_library(WiiExtension 
    WiiExtension.cpp
    extensions/ExtensionBase.cpp
    extensions/ClassicExtension.cpp
    extensions/DrumExtension.cpp
    extensions/GuitarExtension.cpp
    extensions/MotionPlusExtension.cpp
    extensions/NunchuckExtension.cpp
    extensions/TaikoExtension.cpp
    extensions/TurntableExtension.cpp
    extensions/UDrawExtension.cpp
)
target_link_libraries(WiiExtension PUBLIC pico_stdlib PicoPeripherals CRC32)
target_include_directories(WiiExtension INTERFACE .)
target_include_directories(WiiExtension PUBLIC . PicoPeripherals CRC32)
