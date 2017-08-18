set(PROG miniXyce)
list(APPEND CXXFLAGS -DMINIXYCE_INFO=0)
# Single Pass Circuit Simulator.  Runs very quickly.  Unsure how to scale up.
set(RUN_OPTIONS -c ${CMAKE_CURRENT_SOURCE_DIR}/cir5.net -pf ${CMAKE_CURRENT_SOURCE_DIR}/last_used_params.txt)
llvm_multisource()
