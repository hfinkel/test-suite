set(PROG FIR)
list(APPEND LDFLAGS -lm)
list(APPEND CFLAGS -std=c++11)
llvm_multisource()
