set(PROG bullet)
list(APPEND CPPFLAGS -I${CMAKE_CURRENT_SOURCE_DIR}/include -DNO_TIME)
list(APPEND LDFLAGS -lstdc++ -lm)
if(ARCH STREQUAL "XCore")
  set(XCORE_TARGET_NEEDS_MEMORY 64)
endif()
llvm_multisource()
