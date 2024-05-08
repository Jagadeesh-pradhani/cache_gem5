# cache_gem5
Cache memory simulation in gem5


This branch is used for creation of simobject in gem5. <br>

## Steps
   Paste the folder 'newobj' in 'src/learning_gem5/' location. <br>
   Build gem5
   ```
    scons build/X86/gem5.opt -j$(nproc)
   ```

## Testing
   Paste the folder 'cachemini' in 'configs/' location. <br>
   Run the code 'simex.py' to test newly added simobject.<br>
   ```
   build/X86/gem5.opt configs/cachemini/simex.py
   ```

   Modify .cc , .hh and .py files in 'newobj' folder as required for further experimentation.





