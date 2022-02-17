# Usage

```
./nb_binder myBindingDef [minCycle maxCycle]
```

myBindingDef	Nosqlbench binding to test
minCycle	    Starting cycle. Default to 0
maxCycle        Ending cycle. Default to minCycle + 10

for more info on cycle, please visit [Nosqlbench Docs](https://docs.nosqlbench.io/)

# Examples

```
./nb_binder "Identity()"                 #cycles 0 to 10
./nb_binder "HashRange(0,1000)" 100      #cycles 100 to 110
./nb_binder "HashRange(0,1000)" 10 1000  #cycles 10 to 1000
```
