set(MTS_PLUGIN_PREFIX "integrators")

add_plugin(depth   depth.cpp)
add_plugin(direct  direct.cpp)
add_plugin(path    path.cpp)
add_plugin(aov     aov.cpp)
add_plugin(stokes  stokes.cpp)
add_plugin(moment  moment.cpp)
add_plugin(volpath  volpath.cpp)
add_plugin(volpathmis volpathmis.cpp)

add_plugin(path_sms_ss path_sms_ss.cpp)
add_plugin(path_filtered_ss path_filtered_ss.cpp)

add_plugin(path_sms_ms path_sms_ms.cpp)
add_plugin(path_filtered_ms path_filtered_ms.cpp)

add_plugin(path_sms_glints path_sms_glints.cpp)

add_plugin(path_sms_teaser path_sms_teaser.cpp)
add_plugin(path_filtered_teaser path_filtered_teaser.cpp)

# Register the test directory
add_tests(${CMAKE_CURRENT_SOURCE_DIR}/tests)
