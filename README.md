# ANTLR Cmake Starter

## Description

A ready to use starter project using ANTLR with cmake.

There are no dependencies. The script `/tools/antlr/download.sh` will
download ANTLR and it will be used as a CMake dependency.

## Instructions

```bash

# Download ANTLR and build the CPP runtime.
cd tools/antlr
./download.sh
cd ../..

# Build the project
mkdir build
cd build
cmake ..
make
./src/main

```

## Output example

```bash
Please enter an expression (for instance (1+2)*(3-4)/(5-6))
input = 4/2-3*3+1-1
Result = -9
Tree = 
             
             4
            ╱
           ÷ 
          ╱ ╲
         ╱   2
        ╱    
       ╱        
      -         3
     ╱ ╲       ╱
    ╱   ╲     x 
   ╱     ╲   ╱ ╲
  ╱       ╲ ╱   3
 ╱         +    
-           ╲ 
 ╲           ╲
  ╲           1
   ╲          
    ╲ 
     ╲
      1
      
```
