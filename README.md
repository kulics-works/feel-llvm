# feel-llvm

## Use

1. build llvm ir

2. build llvm obj
```
llc -filetype=obj main.ll -o main.o
```
3. link to bin
```
gcc main.o
```

4. link more file
```
llvm-link file1.ll file2.ll -o linked.ir
```

5. test 
```
clang++ test.cpp main.o -o main && ./main
```