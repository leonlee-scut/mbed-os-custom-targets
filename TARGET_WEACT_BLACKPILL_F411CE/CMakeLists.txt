# Copyright (c) 2022 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-weact-blackpill-f411ce INTERFACE)

target_sources(mbed-weact-blackpill-f411ce
    INTERFACE
        PeripheralPins.c
        system_clock_overrides.c
)

target_include_directories(mbed-weact-blackpill-f411ce
    INTERFACE
        .
)

target_link_libraries(mbed-weact-blackpill-f411ce INTERFACE mbed-stm32f411xe)
