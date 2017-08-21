set(PROG CoMD)
list(APPEND CPPFLAGS -DVERIFICATION) 
list(APPEND LDFLAGS -lm)
llvm_multisource()
