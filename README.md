# cache_gem5
Cache memory simulation in gem5


# installation

```
git clone https://github.com/gem5/gem5
```

# Install dependecies
For setup on Ubuntu 22.04 (gem5 >= v21.1)
for other versions: https://www.gem5.org/documentation/general_docs/building
```
sudo apt install build-essential git m4 scons zlib1g zlib1g-dev \
    libprotobuf-dev protobuf-compiler libprotoc-dev libgoogle-perftools-dev \
    python3-dev libboost-all-dev pkg-config python3-tk
```

# Build

```
scons build/X86/gem5.opt
```
or 
```
scons build/ALL/$add binary type
```
or
```
scons build/X86/gem5.opt -j {No. of CPU's}
```

# Codespace

go to https://github.com/gem5/gem5 open codepace and repeat installation.
cloudspace will be used.

## Getting started

A good starting point is <http://www.gem5.org/about>, and for
more information about building the simulator and getting started
please see <http://www.gem5.org/documentation> and
<http://www.gem5.org/documentation/learning_gem5/introduction>.


# Running
Be in gem5 folder<br>

Create a folder in gem5/configs directory.<br>

To create a config script:- https://www.gem5.org/documentation/learning_gem5/part1/simple_config/ <br>
https://www.gem5.org/documentation/learning_gem5/part1/cache_config/

Copy paste the codes in that folder.<br>

To tun the python code,
```
build/X86/gem5.opt configs/folder_name/tcmp.py
```

Output of the simulation will be stored in gem5/m5out folder

# Prefetcher

Source default prefetcher python code:-  "gem5/src/mem/cache/prefetch/Prefetcher.py" <br>

For new prefetcher creation : https://www.gem5.org/documentation/learning_gem5/part2/helloobject/  <br>




