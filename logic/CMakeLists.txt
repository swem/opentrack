opentrack_boilerplate(opentrack-logic BIN)
target_link_libraries(opentrack-logic opentrack-spline-widget)
if(NOT WIN32)
    target_link_libraries(opentrack-logic opentrack-qxt-mini)
else()
    target_link_libraries(opentrack-logic opentrack-dinput winmm)
endif()
