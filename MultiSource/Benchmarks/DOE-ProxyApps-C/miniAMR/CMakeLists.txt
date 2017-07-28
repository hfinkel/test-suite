set(PROG miniAMR)
list(APPEND CPPFLAGS -I.)
list(APPEND LDFLAGS -lm)
set(RUN_OPTIONS --nx 16 --ny 16 --nz 16)
llvm_multisource()
 
