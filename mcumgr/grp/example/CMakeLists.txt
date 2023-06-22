    # Copyright (c) 2023 Nordic Semiconductor ASA
    # SPDX-License-Identifier: Apache-2.0

    # Example management group public API is exposed by MCUmgr API
    # interface, when example management is enabled.
    if(CONFIG_MCUMGR_GRP_EXAMPLE)
      zephyr_library(mgmt_mcumgr_grp_example)
      # The below should be updated with the real name of the file
      zephyr_library_sources(src/<grp_name>_mgmt.c)
      zephyr_library_include_directories(include)
    endif()
