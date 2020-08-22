Testing system performance with and without cache memory using GEM5 simulator


Instaliing Gem5

git clone https://gem5.googlesource.com/public/gem5

cd gem5

scons build/X86/gem5.opt -j <NUMBER OF CPUs ON YOUR PLATFORM>


build/X86/gem5.opt configs/example/se.py  #system emulation script

Installing Micro-Benchmarks

git clone https://github.com/bhagyashreeborate/Gem5-Simulator 

git clone  https://github.com/PolyArch/cs251a-microbench.git

unzip and make all files

Create a test file (basic.py) for basic system (without cache) -> set process to location of micro benchmark 

run basic.py -> stores simulated results in stats.txt ->> File attached results 

run command - build/X86/gem5.opt <file directory of basic.py>

# System with cache
Create a test file (cache_2_level.py) with l1 and l2 caches with sizes as 16kB,16kB and 64kB

run similar to basic 

micro benchmarks used 

from  https://github.com/PolyArch/cs251a-microbench.git -->> lfsr,merge,mm
from  https://github.com/bhagyashreeborate/Gem5-Simulator -->> blocked-matmul


For validating attached results files  
