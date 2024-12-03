# Commands

## Navigate to gem5 folder
Assuming you have cloned the gem5 in home diorectory
```sh
cd ~/gem5
```

## Build
```sh
scons build/X86/gem5.opt -j($nproc)
```

## Run examples
Create a new folder in configs/
```sh
mkdir ~/gem5/configs/project
```
paste the codes `caches.py`, `simple.py` and `tcmp.py` in this folder.

Run
```sh
cd ~/gem5
build/X86/gem5.opt configs/project/simple.py
```
This will run the code simple.py , analyze this code for simulation details

## Run SE.py
```sh
cd ~/gem5/
build/X86/gem5.opt configs/deprecated/example/se.py -c tests/test-progs/hello/bin/x86/linux/hello
```
this will run the default SE script with default configuration, <br>
Analyze se.py code for different options
