[Reproduce Table 1's results]

According to the readme file,

In folder Internal estimation:
    (a) Run estimation_mcd.m to estimate the model under MCD. This step takes about 18 hours.
    (b) Run se and sensitivity.m to produce standard errors and sensitivity moments. This step
    takes about 30 minutes.
    (c) Run Outputs MCD.m to compile and store estimation results.


estimation_mcd.m calls 

```
[X,fval,exitflag,output] = fminsearch(problem);
```

`problem` is defined in `data/inputs_mcd.m`, which specifies the objective function by calling the function `moments` defined in `Internal_estimation/Inputs/moments.m`.

