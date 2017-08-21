set(PROG FIND_FIRST_MIN)
list(APPEND LDFLAGS -lm)
list(APPEND CFLAGS -std=c++11)
llvm_multisource()
