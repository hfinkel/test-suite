set(PROG lcals.exe)
set(Source 
	runBRawLoops.cxx
	runCForallLambdaLoops.cxx
	runOMPRawLoops.cxx
	LCALSStats.cxx
	main.cxx
	runOMPForallLambdaLoops.cxx
	runCRawLoops.cxx
	LCALSSuite.cxx
	runReferenceLoops.cxx
	runBForallLambdaLoops.cxx
	LCALSTraversalMethods.cxx
	runARawLoops.cxx
	runAForallLambdaLoops.cxx
)

list(APPEND LDFLAGS -lm)
list(APPEND CFLAGS -Ofast -mavx -finline-functions -finline-limit=10000 -std=c++11)
list(APPEND CXXFLAGS -I. -DLCALS_PLATFORM_X86_AVX -DLCALS_COMPILER_GNU -DLCALS_USE_DOUBLE -DLCALS_USE_RESTRICT_PTR  -DLCALS_VERIFY_CHECKSUM -DLCALS_USE_CLOCK)
llvm_multisource()
