# LLVM_PASS

## this is a collection of some projects using llvm pass to instrument

**in the folder srciror there is a tool for mutating and analysing coverage**

**in the folder llvm_instru_master there is a project demo**

if use
clang++ -c basic_block_pass.cpp `llvm-config --cxxflags`
clang++ -shared -o pass.so basic_block_pass.o `llvm-config --ldflags`
to compile my pass
then it's necessary to add "-undefined suppress -flat_namespace"

some url may help:
	-https://www.jianshu.com/p/b48c1b482c82?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation
	-https://www.jianshu.com/p/b2f9efea49c3
	-https://www.jianshu.com/p/4d392b16d831
	
notice that in llvm 11. the method getorinsertfunction is no longer a constant class but a fuctioncallee one. Remaining to be solve

