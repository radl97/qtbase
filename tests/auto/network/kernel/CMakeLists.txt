add_subdirectory(qdnslookup)
add_subdirectory(qdnslookup_appless)
add_subdirectory(qnetworkinterface)
add_subdirectory(qnetworkdatagram)
add_subdirectory(qnetworkaddressentry)
add_subdirectory(qhostaddress)

if(NOT WINRT)
    add_subdirectory(qnetworkproxy)
    add_subdirectory(qnetworkproxyfactory)
endif()

if(QT_FEATURE_private_tests)
    add_subdirectory(qauthenticator)

    if(NOT MACOS)
        add_subdirectory(qhostinfo)
    endif()
endif()
