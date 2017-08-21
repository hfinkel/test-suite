set(PROG COUPLE)
list(APPEND LDFLAGS -lm)
list(APPEND CFLAGS -std=c++11)
llvm_multisource()
