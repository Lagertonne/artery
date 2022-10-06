#add_artery_feature(vehicle)
#generate_opp_message(PoliceClearLane.msg TARGET police DIRECTORY police_msgs)
add_opp_run(geometry_spikes NED_FOLDERS ${CMAKE_CURRENT_SOURCE_DIR})

if(WITH_ENVMOD)
    target_link_libraries(envmod PRIVATE)
endif()
