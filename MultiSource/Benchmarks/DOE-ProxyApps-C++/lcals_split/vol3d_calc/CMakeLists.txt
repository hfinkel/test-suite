set(PROG VOL3D_CALC)
list(APPEND LDFLAGS -lm)
list(APPEND CFLAGS -std=c++11)
llvm_multisource()
