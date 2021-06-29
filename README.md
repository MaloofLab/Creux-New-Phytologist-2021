# Creux-New-Phytologist-2021

This repository contains data, code, and figures for Bayesian analysis of style and anther growth presened in Creux et al, New Phytologis.

Folder `input` contains the input data

Folder `scripts` contains the analysis scripts

Folder `output` contains the results

Folder `paper` contains formatted figures and text

## Session Info

```
Show in New Window

── Column specification ───────────────────────────────────────────────────────────────────────────────────
cols(
  Day = col_double(),
  floret = col_double(),
  Treatment = col_character(),
  Time = col_time(format = ""),
  `Length (mm)` = col_double()
)

Show in New Window
── Data Summary ────────────────────────
                           Values    
Name                       Piped data
Number of rows             1224      
Number of columns          7         
_______________________              
Column type frequency:               
  character                1         
  difftime                 1         
  factor                   1         
  numeric                  4         
________________________             
Group variables            None      

── Variable type: character ───────────────────────────────────────────────────────────────────────────────
  skim_variable n_missing complete_rate   min   max empty n_unique whitespace
1 id                    0             1     8    12     0       72          0

── Variable type: difftime ────────────────────────────────────────────────────────────────────────────────
  skim_variable n_missing complete_rate min        max        median     n_unique
1 time                  0             1 19800 secs 34200 secs 27000 secs       17

── Variable type: factor ──────────────────────────────────────────────────────────────────────────────────
  skim_variable n_missing complete_rate ordered n_unique top_counts                  
1 trt                   0             1 FALSE          3 Eas: 408, Wes: 408, Wes: 408

── Variable type: numeric ─────────────────────────────────────────────────────────────────────────────────
  skim_variable n_missing complete_rate  mean    sd    p0   p25   p50   p75  p100 hist 
1 day                   0         1      5.12 2.71   1     2.75  5.5   7.25   9   ▇▃▃▇▇
2 floret                0         1      2    0.817  1     1     2     3      3   ▇▁▇▁▇
3 length              186         0.848  9.36 1.48   6.18  8.20  9.31 10.4   14.0 ▃▇▇▃▁
4 hour                  0         1      2    1.23   0     1     2     3      4   ▇▆▆▆▇
[1] "East"     "West"     "WestHeat"
Show in New Window
Warning: Removed 186 rows containing missing values (geom_point).
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window

Show in New Window

Show in New Window

Show in New Window

Show in New Window

Show in New Window
                prior class        coef group resp dpar nlpar bound       source
 student_t(3, 0, 2.5) sigma                                              default
               (flat)     b                             delta            default
               (flat)     b   Intercept                 delta       (vectorized)
               (flat)     b     trtWest                 delta       (vectorized)
               (flat)     b trtWestHeat                 delta       (vectorized)
 student_t(3, 0, 2.5)    sd                             delta            default
 student_t(3, 0, 2.5)    sd                id           delta       (vectorized)
 student_t(3, 0, 2.5)    sd   Intercept    id           delta       (vectorized)
               (flat)     b                                 k            default
               (flat)     b   Intercept                     k       (vectorized)
               (flat)     b     trtWest                     k       (vectorized)
               (flat)     b trtWestHeat                     k       (vectorized)
 student_t(3, 0, 2.5)    sd                                 k            default
 student_t(3, 0, 2.5)    sd                id               k       (vectorized)
 student_t(3, 0, 2.5)    sd   Intercept    id               k       (vectorized)
               (flat)     b                              Lmax            default
               (flat)     b   Intercept                  Lmax       (vectorized)
               (flat)     b                              Lmin            default
               (flat)     b   Intercept                  Lmin       (vectorized)
Show in New Window
Compiling Stan program...
Start sampling
starting worker pid=76107 on localhost:11119 at 12:58:08.890
starting worker pid=76121 on localhost:11119 at 12:58:09.129
starting worker pid=76135 on localhost:11119 at 12:58:09.348
starting worker pid=76149 on localhost:11119 at 12:58:09.601

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 1).
Chain 1: 
Chain 1: Gradient evaluation took 0.001087 seconds
Chain 1: 1000 transitions using 10 leapfrog steps per transition would take 10.87 seconds.
Chain 1: Adjust your expectations accordingly!
Chain 1: 
Chain 1: 
Chain 1: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 2).
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: 
Chain 2: Gradient evaluation took 0.000662 seconds
Chain 2: 1000 transitions using 10 leapfrog steps per transition would take 6.62 seconds.
Chain 2: Adjust your expectations accordingly!
Chain 2: 
Chain 2: 
Chain 2: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 3).
Chain 3: 
Chain 3: Gradient evaluation took 0.000723 seconds
Chain 3: 1000 transitions using 10 leapfrog steps per transition would take 7.23 seconds.
Chain 3: Adjust your expectations accordingly!
Chain 3: 
Chain 3: 
Chain 3: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 4).
Chain 4: Rejecting initial value:
Chain 4:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 4:   Stan can't start sampling from this initial value.
Chain 4: Rejecting initial value:
Chain 4:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 4:   Stan can't start sampling from this initial value.
Chain 4: 
Chain 4: Gradient evaluation took 0.00086 seconds
Chain 4: 1000 transitions using 10 leapfrog steps per transition would take 8.6 seconds.
Chain 4: Adjust your expectations accordingly!
Chain 4: 
Chain 4: 
Chain 4: Iteration:    1 / 2000 [  0%]  (Warmup)
Chain 1: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 2: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 3: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 1: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 2: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 3: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 4: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 1: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 2: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 3: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 4: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 1: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 2: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 3: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 1: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 1: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 4: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 2: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 2: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 3: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 3: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 4: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 1: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 2: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 3: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 1: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 4: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 4: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 2: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 3: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 1: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 4: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 2: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 3: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 1: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 4: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 2: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 1: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 1: 
Chain 1:  Elapsed Time: 17.694 seconds (Warm-up)
Chain 1:                15.986 seconds (Sampling)
Chain 1:                33.68 seconds (Total)
Chain 1: 
Chain 3: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 4: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 2: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 2: 
Chain 2:  Elapsed Time: 17.407 seconds (Warm-up)
Chain 2:                16.899 seconds (Sampling)
Chain 2:                34.306 seconds (Total)
Chain 2: 
Chain 3: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 3: 
Chain 3:  Elapsed Time: 17.649 seconds (Warm-up)
Chain 3:                17.756 seconds (Sampling)
Chain 3:                35.405 seconds (Total)
Chain 3: 
Chain 4: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 4: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 4: 
Chain 4:  Elapsed Time: 23.21 seconds (Warm-up)
Chain 4:                13.42 seconds (Sampling)
Chain 4:                36.63 seconds (Total)
Chain 4: 
          used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells 4216131 225.2    6937521 370.6         NA  4969379 265.4
Vcells 8915431  68.1   14964384 114.2      16384 12403654  94.7
Show in New Window
 Family: gaussian 
  Links: mu = identity; sigma = identity 
Formula: length2 | cens(censored) ~ Lmax - (Lmax - Lmin) * exp(-(k * hour)^delta) 
         Lmax ~ 1
         Lmin ~ 1
         k ~ 1
         delta ~ 1
   Data: anther (Number of observations: 1224) 
Samples: 4 chains, each with iter = 2000; warmup = 1000; thin = 1;
         total post-warmup samples = 4000

Population-Level Effects: 
                Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
Lmax_Intercept     12.51      0.15    12.24    12.82 1.00     2167     2304
Lmin_Intercept      7.94      0.07     7.79     8.08 1.00     2539     2404
k_Intercept         0.39      0.01     0.37     0.42 1.00     2181     2271
delta_Intercept     2.29      0.14     2.03     2.59 1.00     2254     2127

Family Specific Parameters: 
      Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sigma     1.12      0.02     1.07     1.17 1.00     3041     2272

Samples were drawn using sampling(NUTS). For each parameter, Bulk_ESS
and Tail_ESS are effective sample size measures, and Rhat is the potential
scale reduction factor on split chains (at convergence, Rhat = 1).
          used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells 4258160 227.5    6937521 370.6         NA  6829137 364.8
Vcells 9011615  68.8   50512828 385.4      16384 63141016 481.8
Show in New Window


          used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells 4388888 234.4    6937521 370.6         NA  6937521 370.6
Vcells 9851967  75.2   40410263 308.4      16384 63141016 481.8
R Console
          used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells 4388888 234.4    6937521 370.6         NA  6937521 370.6
Vcells 9851967  75.2   40410263 308.4      16384 63141016 481.8
Show in New Window


           used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells  4572908 244.3    6937521 370.6         NA  6937521 370.6
Vcells 10783056  82.3   40410263 308.4      16384 63141016 481.8
R Console
           used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells  4572908 244.3    6937521 370.6         NA  6937521 370.6
Vcells 10783056  82.3   40410263 308.4      16384 63141016 481.8
Show in New Window
          used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
Ncells 4286391 229.0    6937521 370.6         NA  6937521 370.6
Vcells 9064549  69.2   60381579 460.7      16384 75476557 575.9
Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
Using 10 posterior samples for ppc type 'dens_overlay' by default.
Warning: Censored responses are not shown in 'pp_check'.
R Console


Show in New Window
Warning: It appears as if you have specified a lower bounded prior on a parameter that has no natural lower bound.
If this is really what you want, please specify argument 'lb' of 'set_prior' appropriately.
Warning occurred for prior 
b_delta ~ exponential(0.5)

Compiling Stan program...
Start sampling
starting worker pid=76306 on localhost:11119 at 13:00:33.794
starting worker pid=76320 on localhost:11119 at 13:00:34.073
starting worker pid=76334 on localhost:11119 at 13:00:34.333
starting worker pid=76348 on localhost:11119 at 13:00:34.589

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 1).
Chain 1: Rejecting initial value:
Chain 1:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 1:   Stan can't start sampling from this initial value.
Chain 1: 
Chain 1: Gradient evaluation took 0.000766 seconds
Chain 1: 1000 transitions using 10 leapfrog steps per transition would take 7.66 seconds.
Chain 1: Adjust your expectations accordingly!
Chain 1: 
Chain 1: 
Chain 1: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 2).
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -1.84619, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -1.51963, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -0.609171, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -1.11426, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -1.24104, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -0.099825, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -1.49976, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: Rejecting initial value:
Chain 2:   Error evaluating the log probability at the initial value.
Chain 2: Exception: exponential_lpdf: Random variable is -1.90058, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 2: 
Chain 2: Gradient evaluation took 0.00073 seconds
Chain 2: 1000 transitions using 10 leapfrog steps per transition would take 7.3 seconds.
Chain 2: Adjust your expectations accordingly!
Chain 2: 
Chain 2: 
Chain 2: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 3).
Chain 3: 
Chain 3: Gradient evaluation took 0.002524 seconds
Chain 3: 1000 transitions using 10 leapfrog steps per transition would take 25.24 seconds.
Chain 3: Adjust your expectations accordingly!
Chain 3: 
Chain 3: 
Chain 3: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 4).
Chain 4: Rejecting initial value:
Chain 4:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 4:   Stan can't start sampling from this initial value.
Chain 4: Rejecting initial value:
Chain 4:   Error evaluating the log probability at the initial value.
Chain 4: Exception: exponential_lpdf: Random variable is -0.26906, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 4: Rejecting initial value:
Chain 4:   Error evaluating the log probability at the initial value.
Chain 4: Exception: exponential_lpdf: Random variable is -1.68216, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 4: Rejecting initial value:
Chain 4:   Error evaluating the log probability at the initial value.
Chain 4: Exception: exponential_lpdf: Random variable is -1.23181, but must be nonnegative! (in 'anon_model', line 78, column 2 to column 47)
Chain 4: 
Chain 4: Gradient evaluation took 0.001643 seconds
Chain 4: 1000 transitions using 10 leapfrog steps per transition would take 16.43 seconds.
Chain 4: Adjust your expectations accordingly!
Chain 4: 
Chain 4: 
Chain 4: Iteration:    1 / 5000 [  0%]  (Warmup)
Chain 1: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 4: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 2: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 1: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 2: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 4: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 1: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 2: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 4: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 1: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 2: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 4: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 3: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 1: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 1: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 2: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 2: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 4: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 4: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 3: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 4: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 1: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 3: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 2: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 3: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 4: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 1: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 2: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 3: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 3: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 4: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 1: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 4: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 3: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 2: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 1: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 4: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 4: 
Chain 4:  Elapsed Time: 145.761 seconds (Warm-up)
Chain 4:                119.81 seconds (Sampling)
Chain 4:                265.571 seconds (Total)
Chain 4: 
Chain 3: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 2: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 1: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 1: 
Chain 1:  Elapsed Time: 143.16 seconds (Warm-up)
Chain 1:                141.503 seconds (Sampling)
Chain 1:                284.663 seconds (Total)
Chain 1: 
Chain 3: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 2: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 2: 
Chain 2:  Elapsed Time: 144.213 seconds (Warm-up)
Chain 2:                152.251 seconds (Sampling)
Chain 2:                296.464 seconds (Total)
Chain 2: 
Chain 3: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 3: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 3: 
Chain 3:  Elapsed Time: 214.18 seconds (Warm-up)
Chain 3:                97.019 seconds (Sampling)
Chain 3:                311.199 seconds (Total)
Chain 3: 
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4498318 240.3    6937521 370.6         NA   6937521  370.6
Vcells 11825816  90.3  126399944 964.4      16384 157999363 1205.5
Show in New Window
 Family: gaussian 
  Links: mu = identity; sigma = identity 
Formula: length2 | cens(censored) ~ Lmax - (Lmax - Lmin) * exp(-(k * hour)^delta) 
         Lmax ~ 1
         Lmin ~ 1
         k ~ 1
         delta ~ trt + (1 | id)
   Data: anther (Number of observations: 1224) 
Samples: 4 chains, each with iter = 5000; warmup = 2500; thin = 1;
         total post-warmup samples = 10000

Group-Level Effects: 
~id (Number of levels: 72) 
                    Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(delta_Intercept)     0.97      0.11     0.78     1.20 1.00     1845     3119

Population-Level Effects: 
                  Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
Lmax_Intercept       15.51      0.14    15.22    15.80 1.00     5315     5822
Lmin_Intercept        7.80      0.05     7.70     7.90 1.00     7920     7043
k_Intercept           0.24      0.00     0.23     0.25 1.00     5199     6148
delta_Intercept       1.75      0.19     1.39     2.14 1.00     1240     2378
delta_trtWest         0.19      0.25    -0.29     0.68 1.00     1277     2338
delta_trtWestHeat     0.16      0.24    -0.33     0.63 1.00     1353     2573

Family Specific Parameters: 
      Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sigma     0.77      0.02     0.74     0.81 1.00     7473     7308

Samples were drawn using sampling(NUTS). For each parameter, Bulk_ESS
and Tail_ESS are effective sample size measures, and Rhat is the potential
scale reduction factor on split chains (at convergence, Rhat = 1).
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4498409 240.3    6937521 370.6         NA   6937521  370.6
Vcells 11826074  90.3  101119956 771.5      16384 157999363 1205.5
Show in New Window

           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4689628 250.5    6937521 370.6         NA   6937521  370.6
Vcells 14290147 109.1   80895965 617.2      16384 157999363 1205.5
R Console
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4689628 250.5    6937521 370.6         NA   6937521  370.6
Vcells 14290147 109.1   80895965 617.2      16384 157999363 1205.5
Show in New Window


Using 10 posterior samples for ppc type 'dens_overlay' by default.
Warning: Censored responses are not shown in 'pp_check'.
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`summarise()` has grouped output by 'day', 'trt'. You can override using the `.groups` argument.
R Console


Show in New Window
      elpd_diff se_diff
fit2c    0.0       0.0 
fit1c -376.6      22.1 
Show in New Window
Hypothesis Tests for class b:
---
'CI': 90%-CI for one-sided and 95%-CI for two-sided hypotheses.
'*': For one-sided hypotheses, the posterior probability exceeds 95%;
for two-sided hypotheses, the value tested against lies outside the 95%-CI.
Posterior probabilities of point hypotheses assume equal prior probabilities.
R Console
Description:df [3 × 8]
Hypothesis
<chr>
Estimate
<dbl>
Est.Error
<dbl>
CI.Lower
<dbl>
(delta_trtWest) = 0	0.19	0.25	-0.29	
(delta_trtWestHeat) = 0	0.16	0.24	-0.33	
(delta_trtWest)-(... = 0	0.03	0.27	-0.51	
3 rows | 1-4 of 8 columns
data.frame
3 x 8
Description:df [3 × 8]
Hypothesis
<chr>
Estimate
<dbl>
Est.Error
<dbl>
CI.Lower
<dbl>
(delta_trtWest) = 0	0.19	0.25	-0.29	
(delta_trtWestHeat) = 0	0.16	0.24	-0.33	
(delta_trtWest)-(... = 0	0.03	0.27	-0.51	
3 rows | 1-4 of 8 columns
Show in New Window
Warning: It appears as if you have specified a lower bounded prior on a parameter that has no natural lower bound.
If this is really what you want, please specify argument 'lb' of 'set_prior' appropriately.
Warning occurred for prior 
b_k ~ exponential(1)
b_delta ~ exponential(0.5)

Compiling Stan program...
Start sampling
starting worker pid=76542 on localhost:11119 at 13:07:47.250
starting worker pid=76556 on localhost:11119 at 13:07:47.528
starting worker pid=76570 on localhost:11119 at 13:07:47.766
starting worker pid=76584 on localhost:11119 at 13:07:48.013

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 1).
Chain 1: 
Chain 1: Gradient evaluation took 0.000538 seconds
Chain 1: 1000 transitions using 10 leapfrog steps per transition would take 5.38 seconds.
Chain 1: Adjust your expectations accordingly!
Chain 1: 
Chain 1: 
Chain 1: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 2).
Chain 2: 
Chain 2: Gradient evaluation took 0.0036 seconds
Chain 2: 1000 transitions using 10 leapfrog steps per transition would take 36 seconds.
Chain 2: Adjust your expectations accordingly!
Chain 2: 
Chain 2: 
Chain 2: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 3).
Chain 3: 
Chain 3: Gradient evaluation took 0.001676 seconds
Chain 3: 1000 transitions using 10 leapfrog steps per transition would take 16.76 seconds.
Chain 3: Adjust your expectations accordingly!
Chain 3: 
Chain 3: 
Chain 3: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 4).
Chain 4: 
Chain 4: Gradient evaluation took 0.000881 seconds
Chain 4: 1000 transitions using 10 leapfrog steps per transition would take 8.81 seconds.
Chain 4: Adjust your expectations accordingly!
Chain 4: 
Chain 4: 
Chain 4: Iteration:    1 / 5000 [  0%]  (Warmup)
Chain 3: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 4: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 1: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 2: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 3: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 4: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 1: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 2: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 3: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 4: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 1: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 2: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 3: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 4: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 1: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 2: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 3: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 3: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 4: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 4: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 1: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 1: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 2: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 2: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 3: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 1: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 2: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 4: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 3: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 1: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 2: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 3: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 1: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 4: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 2: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 3: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 1: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 2: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 4: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 3: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 3: 
Chain 3:  Elapsed Time: 262.764 seconds (Warm-up)
Chain 3:                191.639 seconds (Sampling)
Chain 3:                454.403 seconds (Total)
Chain 3: 
Chain 1: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 1: 
Chain 1:  Elapsed Time: 276.656 seconds (Warm-up)
Chain 1:                187.693 seconds (Sampling)
Chain 1:                464.349 seconds (Total)
Chain 1: 
Chain 2: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 2: 
Chain 2:  Elapsed Time: 280.082 seconds (Warm-up)
Chain 2:                190.691 seconds (Sampling)
Chain 2:                470.773 seconds (Total)
Chain 2: 
Chain 4: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 4: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 4: 
Chain 4:  Elapsed Time: 273.483 seconds (Warm-up)
Chain 4:                220.496 seconds (Sampling)
Chain 4:                493.979 seconds (Total)
Chain 4: 
           used  (Mb) gc trigger   (Mb) limit (Mb)  max used   (Mb)
Ncells  4720647 252.2    6937521  370.6         NA   6937521  370.6
Vcells 15303922 116.8  138496461 1056.7      16384 173119397 1320.8
Show in New Window
 Family: gaussian 
  Links: mu = identity; sigma = identity 
Formula: length2 | cens(censored) ~ Lmax - (Lmax - Lmin) * exp(-(k * hour)^delta) 
         Lmax ~ 1
         Lmin ~ 1
         delta ~ 1
         k ~ trt + (1 | id)
   Data: anther (Number of observations: 1224) 
Samples: 4 chains, each with iter = 5000; warmup = 2500; thin = 1;
         total post-warmup samples = 10000

Group-Level Effects: 
~id (Number of levels: 72) 
                Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(k_Intercept)     0.13      0.01     0.11     0.16 1.00     1060     2298

Population-Level Effects: 
                Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
Lmax_Intercept     13.15      0.12    12.93    13.40 1.00     5403     5601
Lmin_Intercept      7.78      0.05     7.68     7.88 1.00     6050     6812
delta_Intercept     1.95      0.08     1.80     2.12 1.00     4847     6181
k_Intercept         0.37      0.02     0.34     0.41 1.01      695     1735
k_trtWest          -0.01      0.02    -0.04     0.03 1.00     1557     3077
k_trtWestHeat      -0.00      0.02    -0.04     0.03 1.00     1786     3598

Family Specific Parameters: 
      Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sigma     0.72      0.02     0.69     0.75 1.00     8514     7420

Samples were drawn using sampling(NUTS). For each parameter, Bulk_ESS
and Tail_ESS are effective sample size measures, and Rhat is the potential
scale reduction factor on split chains (at convergence, Rhat = 1).
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4720712 252.2    6937521 370.6         NA   6937521  370.6
Vcells 15304127 116.8  110797169 845.4      16384 173119397 1320.8
Show in New Window



Show in New Window

           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4913619 262.5    9099172 486.0         NA   6937521  370.6
Vcells 17821208 136.0   70910189 541.1      16384 173119397 1320.8
R Console
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4913619 262.5    9099172 486.0         NA   6937521  370.6
Vcells 17821208 136.0   70910189 541.1      16384 173119397 1320.8
Show in New Window


Using 10 posterior samples for ppc type 'dens_overlay' by default.
Warning: Censored responses are not shown in 'pp_check'.
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`summarise()` has grouped output by 'day', 'trt'. You can override using the `.groups` argument.
R Console


Show in New Window
      elpd_diff se_diff
fit3c    0.0       0.0 
fit2c  -81.6      19.2 
fit1c -458.2      24.0 
Show in New Window
Warning: It appears as if you have specified a lower bounded prior on a parameter that has no natural lower bound.
If this is really what you want, please specify argument 'lb' of 'set_prior' appropriately.
Warning occurred for prior 
b_k ~ exponential(1)
b_delta ~ exponential(0.5)

Compiling Stan program...
Start sampling
starting worker pid=76837 on localhost:11119 at 13:18:05.011
starting worker pid=76851 on localhost:11119 at 13:18:05.276
starting worker pid=76865 on localhost:11119 at 13:18:05.520
starting worker pid=76879 on localhost:11119 at 13:18:05.768

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 1).
Chain 1: 
Chain 1: Gradient evaluation took 0.000894 seconds
Chain 1: 1000 transitions using 10 leapfrog steps per transition would take 8.94 seconds.
Chain 1: Adjust your expectations accordingly!
Chain 1: 
Chain 1: 
Chain 1: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 2).
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: 
Chain 2: Gradient evaluation took 0.000906 seconds
Chain 2: 1000 transitions using 10 leapfrog steps per transition would take 9.06 seconds.
Chain 2: Adjust your expectations accordingly!
Chain 2: 
Chain 2: 
Chain 2: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 3).
Chain 3: 
Chain 3: Gradient evaluation took 0.000832 seconds
Chain 3: 1000 transitions using 10 leapfrog steps per transition would take 8.32 seconds.
Chain 3: Adjust your expectations accordingly!
Chain 3: 
Chain 3: 
Chain 3: Iteration:    1 / 5000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 4).
Chain 4: Rejecting initial value:
Chain 4:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 4:   Stan can't start sampling from this initial value.
Chain 4: Rejecting initial value:
Chain 4:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 4:   Stan can't start sampling from this initial value.
Chain 4: 
Chain 4: Gradient evaluation took 0.012245 seconds
Chain 4: 1000 transitions using 10 leapfrog steps per transition would take 122.45 seconds.
Chain 4: Adjust your expectations accordingly!
Chain 4: 
Chain 4: 
Chain 4: Iteration:    1 / 5000 [  0%]  (Warmup)
Chain 3: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 2: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 1: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 4: Iteration:  500 / 5000 [ 10%]  (Warmup)
Chain 3: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 2: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 1: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 4: Iteration: 1000 / 5000 [ 20%]  (Warmup)
Chain 3: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 1: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 2: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 4: Iteration: 1500 / 5000 [ 30%]  (Warmup)
Chain 1: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 3: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 2: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 4: Iteration: 2000 / 5000 [ 40%]  (Warmup)
Chain 1: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 1: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 2: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 2: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 3: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 3: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 4: Iteration: 2500 / 5000 [ 50%]  (Warmup)
Chain 4: Iteration: 2501 / 5000 [ 50%]  (Sampling)
Chain 1: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 2: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 3: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 4: Iteration: 3000 / 5000 [ 60%]  (Sampling)
Chain 1: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 2: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 3: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 4: Iteration: 3500 / 5000 [ 70%]  (Sampling)
Chain 1: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 2: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 3: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 4: Iteration: 4000 / 5000 [ 80%]  (Sampling)
Chain 1: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 2: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 3: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 4: Iteration: 4500 / 5000 [ 90%]  (Sampling)
Chain 1: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 1: 
Chain 1:  Elapsed Time: 330.179 seconds (Warm-up)
Chain 1:                235.254 seconds (Sampling)
Chain 1:                565.433 seconds (Total)
Chain 1: 
Chain 2: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 2: 
Chain 2:  Elapsed Time: 332.767 seconds (Warm-up)
Chain 2:                234.393 seconds (Sampling)
Chain 2:                567.16 seconds (Total)
Chain 2: 
Chain 3: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 3: 
Chain 3:  Elapsed Time: 331.984 seconds (Warm-up)
Chain 3:                236.42 seconds (Sampling)
Chain 3:                568.404 seconds (Total)
Chain 3: 
Chain 4: Iteration: 5000 / 5000 [100%]  (Sampling)
Chain 4: 
Chain 4:  Elapsed Time: 333.266 seconds (Warm-up)
Chain 4:                235.153 seconds (Sampling)
Chain 4:                568.419 seconds (Total)
Chain 4: 
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  4924736 263.1    9099172 486.0         NA   9099172  486.0
Vcells 19376727 147.9  121404308 926.3      16384 189693904 1447.3
Show in New Window
 Family: gaussian 
  Links: mu = identity; sigma = identity 
Formula: length2 | cens(censored) ~ Lmax - (Lmax - Lmin) * exp(-(k * hour)^delta) 
         Lmax ~ 1
         Lmin ~ 1
         delta ~ trt + (1 | id)
         k ~ trt + (1 | id)
   Data: anther (Number of observations: 1224) 
Samples: 4 chains, each with iter = 5000; warmup = 2500; thin = 1;
         total post-warmup samples = 10000

Group-Level Effects: 
~id (Number of levels: 72) 
                    Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(delta_Intercept)     0.58      0.09     0.42     0.76 1.00     3963     6578
sd(k_Intercept)         0.12      0.01     0.10     0.14 1.00     2479     4528

Population-Level Effects: 
                  Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
Lmax_Intercept       13.40      0.13    13.15    13.67 1.00     9347     8262
Lmin_Intercept        7.76      0.05     7.68     7.85 1.00    16916     7639
delta_Intercept       1.79      0.14     1.53     2.08 1.00     5701     6731
delta_trtWest         0.29      0.16    -0.03     0.60 1.00     6782     7010
delta_trtWestHeat     0.35      0.16     0.03     0.64 1.00     6536     7190
k_Intercept           0.36      0.02     0.32     0.39 1.00     1951     4043
k_trtWest            -0.00      0.02    -0.04     0.03 1.00     3971     6113
k_trtWestHeat        -0.00      0.02    -0.03     0.03 1.00     3906     6122

Family Specific Parameters: 
      Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sigma     0.67      0.02     0.64     0.70 1.00    13486     6615

Samples were drawn using sampling(NUTS). For each parameter, Bulk_ESS
and Tail_ESS are effective sample size measures, and Rhat is the potential
scale reduction factor on split chains (at convergence, Rhat = 1).
           used  (Mb) gc trigger (Mb) limit (Mb)  max used   (Mb)
Ncells  4924796 263.1    9099172  486         NA   9099172  486.0
Vcells 19376968 147.9   97123447  741      16384 189693904 1447.3
Show in New Window



Show in New Window

           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5099113 272.4    9099172 486.0         NA   9099172  486.0
Vcells 22025898 168.1   77698758 592.8      16384 189693904 1447.3
R Console
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5099113 272.4    9099172 486.0         NA   9099172  486.0
Vcells 22025898 168.1   77698758 592.8      16384 189693904 1447.3
Show in New Window


Using 10 posterior samples for ppc type 'dens_overlay' by default.
Warning: Censored responses are not shown in 'pp_check'.
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`summarise()` has grouped output by 'trt'. You can override using the `.groups` argument.
R Console


Show in New Window
`summarise()` has grouped output by 'day', 'trt'. You can override using the `.groups` argument.
R Console


Show in New Window
       elpd_diff se_diff
fit_4c    0.0       0.0 
fit3c   -68.5       9.8 
fit2c  -150.1      19.2 
fit1c  -526.7      26.1 
Show in New Window
Warning: It appears as if you have specified a lower bounded prior on a parameter that has no natural lower bound.
If this is really what you want, please specify argument 'lb' of 'set_prior' appropriately.
Warning occurred for prior 
b_k ~ exponential(1)
b_delta ~ exponential(0.5)

Compiling Stan program...
Start sampling
starting worker pid=77180 on localhost:11119 at 13:30:40.708
starting worker pid=77195 on localhost:11119 at 13:30:41.020
starting worker pid=77209 on localhost:11119 at 13:30:41.363
starting worker pid=77224 on localhost:11119 at 13:30:41.846

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 1).
Chain 1: 
Chain 1: Gradient evaluation took 0.001087 seconds
Chain 1: 1000 transitions using 10 leapfrog steps per transition would take 10.87 seconds.
Chain 1: Adjust your expectations accordingly!
Chain 1: 
Chain 1: 
Chain 1: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 2).
Chain 2: 
Chain 2: Gradient evaluation took 0.001937 seconds
Chain 2: 1000 transitions using 10 leapfrog steps per transition would take 19.37 seconds.
Chain 2: Adjust your expectations accordingly!
Chain 2: 
Chain 2: 
Chain 2: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 3).
Chain 3: Rejecting initial value:
Chain 3:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 3:   Stan can't start sampling from this initial value.
Chain 3: 
Chain 3: Gradient evaluation took 0.065723 seconds
Chain 3: 1000 transitions using 10 leapfrog steps per transition would take 657.23 seconds.
Chain 3: Adjust your expectations accordingly!
Chain 3: 
Chain 3: 
Chain 3: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 4).
Chain 4: 
Chain 4: Gradient evaluation took 0.00087 seconds
Chain 4: 1000 transitions using 10 leapfrog steps per transition would take 8.7 seconds.
Chain 4: Adjust your expectations accordingly!
Chain 4: 
Chain 4: 
Chain 4: Iteration:    1 / 2000 [  0%]  (Warmup)
Chain 2: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 3: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 1: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 4: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 2: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 4: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 1: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 3: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 2: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 4: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 1: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 3: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 2: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 4: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 3: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 1: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 2: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 2: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 4: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 4: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 3: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 3: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 1: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 1: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 4: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 3: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 1: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 2: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 4: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 3: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 1: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 4: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 2: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 3: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 1: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 4: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 1: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 3: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 2: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 4: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 4: 
Chain 4:  Elapsed Time: 254.161 seconds (Warm-up)
Chain 4:                97.843 seconds (Sampling)
Chain 4:                352.004 seconds (Total)
Chain 4: 
Chain 1: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 1: 
Chain 1:  Elapsed Time: 266.991 seconds (Warm-up)
Chain 1:                98.1 seconds (Sampling)
Chain 1:                365.091 seconds (Total)
Chain 1: 
Chain 3: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 3: 
Chain 3:  Elapsed Time: 259.674 seconds (Warm-up)
Chain 3:                104.776 seconds (Sampling)
Chain 3:                364.45 seconds (Total)
Chain 3: 
Chain 2: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 2: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 2: 
Chain 2:  Elapsed Time: 253.592 seconds (Warm-up)
Chain 2:                126.031 seconds (Sampling)
Chain 2:                379.623 seconds (Total)
Chain 2: 
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5130163 274.0    9099172 486.0         NA   9099172  486.0
Vcells 21717648 165.7  119569895 912.3      16384 189693904 1447.3
Show in New Window
 Family: gaussian 
  Links: mu = identity; sigma = identity 
Formula: length2 | cens(censored) ~ Lmax - (Lmax - Lmin) * exp(-(k * hour)^delta) 
         Lmin ~ 1
         Lmax ~ (1 | day)
         delta ~ trt + (1 | id)
         k ~ trt + (1 | id)
   Data: anther (Number of observations: 1224) 
Samples: 4 chains, each with iter = 2000; warmup = 1000; thin = 1;
         total post-warmup samples = 4000

Group-Level Effects: 
~day (Number of levels: 8) 
                   Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(Lmax_Intercept)     2.75      0.81     1.55     4.65 1.00      729     1196

~id (Number of levels: 72) 
                    Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(delta_Intercept)     0.67      0.11     0.48     0.91 1.00      875     1567
sd(k_Intercept)         0.04      0.01     0.03     0.05 1.00      987     2173

Population-Level Effects: 
                  Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
Lmin_Intercept        7.73      0.05     7.63     7.82 1.00     3804     3102
Lmax_Intercept       11.65      0.26    11.14    12.14 1.00     1669     1936
delta_Intercept       1.76      0.16     1.47     2.08 1.00     1018     1553
delta_trtWest         0.23      0.17    -0.09     0.56 1.00     1182     2008
delta_trtWestHeat     0.30      0.17    -0.04     0.62 1.00     1244     1628
k_Intercept           0.33      0.02     0.28     0.36 1.00      893     1650
k_trtWest            -0.00      0.01    -0.03     0.02 1.00     1747     2496
k_trtWestHeat         0.00      0.01    -0.02     0.03 1.00     1594     2321

Family Specific Parameters: 
      Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sigma     0.66      0.02     0.64     0.69 1.00     3332     2873

Samples were drawn using sampling(NUTS). For each parameter, Bulk_ESS
and Tail_ESS are effective sample size measures, and Rhat is the potential
scale reduction factor on split chains (at convergence, Rhat = 1).
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5130222 274.0    9099172 486.0         NA   9099172  486.0
Vcells 21717889 165.7   95655916 729.8      16384 189693904 1447.3
Show in New Window

           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5316379 284.0    9099172 486.0         NA   9099172  486.0
Vcells 23223721 177.2   76524733 583.9      16384 189693904 1447.3
R Console
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5316379 284.0    9099172 486.0         NA   9099172  486.0
Vcells 23223721 177.2   76524733 583.9      16384 189693904 1447.3
Show in New Window


Using 10 posterior samples for ppc type 'dens_overlay' by default.
Warning: Censored responses are not shown in 'pp_check'.
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`summarise()` has grouped output by 'trt'. You can override using the `.groups` argument.
R Console


Show in New Window
`summarise()` has grouped output by 'day', 'trt'. You can override using the `.groups` argument.
R Console


Show in New Window
       elpd_diff se_diff
fit_5c    0.0       0.0 
fit_4c  -21.9       6.7 
fit3c   -90.4      13.0 
fit2c  -172.0      21.1 
fit1c  -548.6      28.0 
Show in New Window
Warning: It appears as if you have specified a lower bounded prior on a parameter that has no natural lower bound.
If this is really what you want, please specify argument 'lb' of 'set_prior' appropriately.
Warning occurred for prior 
b_k ~ exponential(1)
b_delta ~ exponential(0.5)

Compiling Stan program...
Start sampling
starting worker pid=77463 on localhost:11119 at 13:39:02.227
starting worker pid=77477 on localhost:11119 at 13:39:02.504
starting worker pid=77491 on localhost:11119 at 13:39:02.754
starting worker pid=77505 on localhost:11119 at 13:39:03.012

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 1).
Chain 1: Rejecting initial value:
Chain 1:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 1:   Stan can't start sampling from this initial value.
Chain 1: 
Chain 1: Gradient evaluation took 0.001143 seconds
Chain 1: 1000 transitions using 10 leapfrog steps per transition would take 11.43 seconds.
Chain 1: Adjust your expectations accordingly!
Chain 1: 
Chain 1: 
Chain 1: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 2).
Chain 2: Rejecting initial value:
Chain 2:   Log probability evaluates to log(0), i.e. negative infinity.
Chain 2:   Stan can't start sampling from this initial value.
Chain 2: 
Chain 2: Gradient evaluation took 0.001321 seconds
Chain 2: 1000 transitions using 10 leapfrog steps per transition would take 13.21 seconds.
Chain 2: Adjust your expectations accordingly!
Chain 2: 
Chain 2: 
Chain 2: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 3).
Chain 3: 
Chain 3: Gradient evaluation took 0.001497 seconds
Chain 3: 1000 transitions using 10 leapfrog steps per transition would take 14.97 seconds.
Chain 3: Adjust your expectations accordingly!
Chain 3: 
Chain 3: 
Chain 3: Iteration:    1 / 2000 [  0%]  (Warmup)

SAMPLING FOR MODEL 'anon_model' NOW (CHAIN 4).
Chain 4: 
Chain 4: Gradient evaluation took 0.001221 seconds
Chain 4: 1000 transitions using 10 leapfrog steps per transition would take 12.21 seconds.
Chain 4: Adjust your expectations accordingly!
Chain 4: 
Chain 4: 
Chain 4: Iteration:    1 / 2000 [  0%]  (Warmup)
Chain 3: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 4: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 2: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 1: Iteration:  200 / 2000 [ 10%]  (Warmup)
Chain 3: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 4: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 2: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 1: Iteration:  400 / 2000 [ 20%]  (Warmup)
Chain 4: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 3: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 1: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 2: Iteration:  600 / 2000 [ 30%]  (Warmup)
Chain 4: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 3: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 1: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 2: Iteration:  800 / 2000 [ 40%]  (Warmup)
Chain 4: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 4: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 3: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 3: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 1: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 1: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 2: Iteration: 1000 / 2000 [ 50%]  (Warmup)
Chain 2: Iteration: 1001 / 2000 [ 50%]  (Sampling)
Chain 4: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 3: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 1: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 2: Iteration: 1200 / 2000 [ 60%]  (Sampling)
Chain 4: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 3: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 1: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 2: Iteration: 1400 / 2000 [ 70%]  (Sampling)
Chain 4: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 3: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 1: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 2: Iteration: 1600 / 2000 [ 80%]  (Sampling)
Chain 4: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 3: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 1: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 4: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 4: 
Chain 4:  Elapsed Time: 224.159 seconds (Warm-up)
Chain 4:                84.721 seconds (Sampling)
Chain 4:                308.88 seconds (Total)
Chain 4: 
Chain 2: Iteration: 1800 / 2000 [ 90%]  (Sampling)
Chain 3: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 3: 
Chain 3:  Elapsed Time: 230.212 seconds (Warm-up)
Chain 3:                83.288 seconds (Sampling)
Chain 3:                313.5 seconds (Total)
Chain 3: 
Chain 1: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 1: 
Chain 1:  Elapsed Time: 241.278 seconds (Warm-up)
Chain 1:                79.375 seconds (Sampling)
Chain 1:                320.653 seconds (Total)
Chain 1: 
Chain 2: Iteration: 2000 / 2000 [100%]  (Sampling)
Chain 2: 
Chain 2:  Elapsed Time: 242.74 seconds (Warm-up)
Chain 2:                78.142 seconds (Sampling)
Chain 2:                320.882 seconds (Total)
Chain 2: 
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5334636 285.0    9099172 486.0         NA   9099172  486.0
Vcells 24170397 184.5   76615362 584.6      16384 189693904 1447.3
Show in New Window
 Family: gaussian 
  Links: mu = identity; sigma = identity 
Formula: length2 | cens(censored) ~ Lmax - (Lmax - Lmin) * exp(-(k * hour)^delta) 
         Lmax ~ (1 | day)
         Lmin ~ (1 | day)
         delta ~ trt + (1 | id)
         k ~ trt + (1 | id)
   Data: anther (Number of observations: 1224) 
Samples: 4 chains, each with iter = 2000; warmup = 1000; thin = 1;
         total post-warmup samples = 4000

Group-Level Effects: 
~day (Number of levels: 8) 
                   Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(Lmax_Intercept)     2.47      0.72     1.39     4.16 1.00     1024     1532
sd(Lmin_Intercept)     0.61      0.22     0.33     1.14 1.00      970     1719

~id (Number of levels: 72) 
                    Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sd(delta_Intercept)     0.49      0.10     0.32     0.71 1.00      949     1722
sd(k_Intercept)         0.04      0.01     0.03     0.05 1.00     1013     1946

Population-Level Effects: 
                  Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
Lmax_Intercept       11.66      0.24    11.17    12.15 1.00     1903     2592
Lmin_Intercept        7.71      0.17     7.36     8.02 1.00     1069     2003
delta_Intercept       1.76      0.15     1.48     2.06 1.00     1206     1981
delta_trtWest         0.35      0.15     0.06     0.64 1.00     1950     2516
delta_trtWestHeat     0.41      0.15     0.10     0.69 1.00     1799     2631
k_Intercept           0.34      0.02     0.29     0.38 1.00      948     1398
k_trtWest            -0.00      0.01    -0.03     0.02 1.00     1415     2297
k_trtWestHeat         0.00      0.01    -0.03     0.03 1.00     1443     1947

Family Specific Parameters: 
      Estimate Est.Error l-95% CI u-95% CI Rhat Bulk_ESS Tail_ESS
sigma     0.64      0.02     0.61     0.67 1.00     2616     2625

Samples were drawn using sampling(NUTS). For each parameter, Bulk_ESS
and Tail_ESS are effective sample size measures, and Rhat is the potential
scale reduction factor on split chains (at convergence, Rhat = 1).
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5334708 285.0    9099172 486.0         NA   9099172  486.0
Vcells 24170671 184.5   76615362 584.6      16384 189693904 1447.3
Show in New Window


           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5538949 295.9    9099172 486.0         NA   9099172  486.0
Vcells 25827427 197.1   76615362 584.6      16384 189693904 1447.3
R Console
           used  (Mb) gc trigger  (Mb) limit (Mb)  max used   (Mb)
Ncells  5538949 295.9    9099172 486.0         NA   9099172  486.0
Vcells 25827427 197.1   76615362 584.6      16384 189693904 1447.3
Show in New Window


Using 10 posterior samples for ppc type 'dens_overlay' by default.
Warning: Censored responses are not shown in 'pp_check'.
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
Warning: Removed 186 rows containing non-finite values (stat_smooth).
`geom_smooth()` using method = 'loess' and formula 'y ~ x'
R Console


Show in New Window
`summarise()` has grouped output by 'day', 'trt'. You can override using the `.groups` argument.
Warning: Removed 62 rows containing missing values (geom_point).
Warning: Removed 62 rows containing missing values (geom_point).
R Console


Show in New Window
       elpd_diff se_diff
fit_6c    0.0       0.0 
fit_5c  -41.2      13.3 
fit_4c  -63.1      14.7 
fit3c  -131.6      17.1 
fit2c  -213.2      21.4 
fit1c  -589.8      27.2 
Show in New Window
         b_Lmax_Intercept          b_Lmin_Intercept         b_delta_Intercept           b_delta_trtWest 
            11.6603550955              7.7107106754              1.7572125610              0.3480487032 
      b_delta_trtWestHeat             b_k_Intercept               b_k_trtWest           b_k_trtWestHeat 
             0.4085974213              0.3366791988             -0.0043306062              0.0021603672 
             prior_b_Lmax              prior_b_Lmin   prior_b_delta_Intercept     prior_b_delta_trtWest 
            11.4986398949              7.4999693078              2.0273121585             -0.0011335972 
prior_b_delta_trtWestHeat       prior_b_k_Intercept         prior_b_k_trtWest     prior_b_k_trtWestHeat 
            -0.0038707272              1.0067453076              0.0003744252              0.0011928831 
           infl_intercept              infl_trtWest          infl_trtWestHeat 
             1.8181198665              2.2064981348              2.2098722873 
Show in New Window
[1] 0.99
Show in New Window
[1] 0.991
Show in New Window
[1] 0.49175
Show in New Window
[1] 0.43225
[1] 0.43225
Show in New Window
[1] 0.62575
[1] 0.62575
Show in New Window
[1] 0.701
Show in New Window

Show in New Window


R version 4.1.0 (2021-05-18) -- "Camp Pontanezen"
Copyright (C) 2021 The R Foundation for Statistical Computing
Platform: x86_64-apple-darwin17.0 (64-bit)

R is free software and comes with ABSOLUTELY NO WARRANTY.
You are welcome to redistribute it under certain conditions.
Type 'license()' or 'licence()' for distribution details.

  Natural language support but running in an English locale

R is a collaborative project with many contributors.
Type 'contributors()' for more information and
'citation()' on how to cite R or R packages in publications.

Type 'demo()' for some demos, 'help()' for on-line help, or
'help.start()' for an HTML browser interface to help.
Type 'q()' to quit R.

> library(tidyverse)
Registered S3 methods overwritten by 'dbplyr':
  method         from
  print.tbl_lazy     
  print.tbl_sql      
── Attaching packages ───────────────────────────── tidyverse 1.3.1 ──
✓ ggplot2 3.3.3     ✓ purrr   0.3.4
✓ tibble  3.1.2     ✓ dplyr   1.0.6
✓ tidyr   1.1.3     ✓ stringr 1.4.0
✓ readr   1.4.0     ✓ forcats 0.5.1
── Conflicts ──────────────────────────────── tidyverse_conflicts() ──
x dplyr::filter() masks stats::filter()
x dplyr::lag()    masks stats::lag()
> library(skimr)
> library(brms)
Loading required package: Rcpp
Registered S3 method overwritten by 'htmlwidgets':
  method           from         
  print.htmlwidget tools:rstudio
Loading 'brms' package (version 2.15.7). Useful instructions
can be found by typing help('brms'). A more detailed introduction
to the package is available through vignette('brms_overview').

Attaching package: ‘brms’

The following object is masked from ‘package:stats’:

    ar

> ?require
> library(tidyverse)
> library(skimr)
> library(brms)
> # you also need package rethinking although it isn't loaded
> library(rethinking)
Loading required package: rstan
Loading required package: StanHeaders

rstan version 2.26.1 (Stan version 2.26.1)

For execution on a local, multicore CPU with excess RAM we recommend calling
options(mc.cores = parallel::detectCores()).
To avoid recompilation of unchanged Stan programs, we recommend calling
rstan_options(auto_write = TRUE)
For within-chain threading using `reduce_sum()` or `map_rect()` Stan functions,
change `threads_per_chain` option:
rstan_options(threads_per_chain = 1)


Attaching package: ‘rstan’

The following object is masked from ‘package:tidyr’:

    extract

Loading required package: parallel
rethinking (Version 2.13)

Attaching package: ‘rethinking’

The following objects are masked from ‘package:brms’:

    LOO, stancode, WAIC

The following object is masked from ‘package:purrr’:

    map

The following object is masked from ‘package:stats’:

    rstudent

> sessionInfo()
R version 4.1.0 (2021-05-18)
Platform: x86_64-apple-darwin17.0 (64-bit)
Running under: macOS Big Sur 11.4

Matrix products: default
LAPACK: /Library/Frameworks/R.framework/Versions/4.1/Resources/lib/libRlapack.dylib

locale:
[1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8

attached base packages:
[1] parallel  stats     graphics  grDevices utils     datasets  methods  
[8] base     

other attached packages:
 [1] rethinking_2.13    rstan_2.26.1       StanHeaders_2.26.1
 [4] brms_2.15.7        Rcpp_1.0.6         skimr_2.1.3       
 [7] forcats_0.5.1      stringr_1.4.0      dplyr_1.0.6       
[10] purrr_0.3.4        readr_1.4.0        tidyr_1.1.3       
[13] tibble_3.1.2       ggplot2_3.3.3      tidyverse_1.3.1   

loaded via a namespace (and not attached):
  [1] readxl_1.3.1         backports_1.2.1      plyr_1.8.6          
  [4] igraph_1.2.6         repr_1.1.3           splines_4.1.0       
  [7] crosstalk_1.1.1      TH.data_1.0-10       rstantools_2.1.1    
 [10] inline_0.3.19        digest_0.6.27        htmltools_0.5.1.1   
 [13] rsconnect_0.8.18     fansi_0.5.0          magrittr_2.0.1      
 [16] modelr_0.1.8         RcppParallel_5.1.4   matrixStats_0.59.0  
 [19] xts_0.12.1           sandwich_3.0-1       prettyunits_1.1.1   
 [22] colorspace_2.0-1     rvest_1.0.0          haven_2.4.1         
 [25] xfun_0.23            callr_3.7.0          crayon_1.4.1        
 [28] jsonlite_1.7.2       lme4_1.1-27          survival_3.2-11     
 [31] zoo_1.8-9            glue_1.4.2           gtable_0.3.0        
 [34] emmeans_1.6.1        V8_3.4.2             pkgbuild_1.2.0      
 [37] shape_1.4.6          abind_1.4-5          scales_1.1.1        
 [40] mvtnorm_1.1-1        DBI_1.1.1            miniUI_0.1.1.1      
 [43] xtable_1.8-4         stats4_4.1.0         DT_0.18             
 [46] htmlwidgets_1.5.3    httr_1.4.2           threejs_0.3.3       
 [49] ellipsis_0.3.2       pkgconfig_2.0.3      loo_2.4.1           
 [52] sass_0.4.0           dbplyr_2.1.1         utf8_1.2.1          
 [55] tidyselect_1.1.1     rlang_0.4.11.9000    reshape2_1.4.4      
 [58] later_1.2.0          munsell_0.5.0        cellranger_1.1.0    
 [61] tools_4.1.0          cli_2.5.0            generics_0.1.0      
 [64] broom_0.7.6          ggridges_0.5.3       evaluate_0.14       
 [67] fastmap_1.1.0        yaml_2.2.1           processx_3.5.2      
 [70] knitr_1.33           fs_1.5.0             nlme_3.1-152        
 [73] mime_0.10            projpred_2.0.2       xml2_1.3.2          
 [76] compiler_4.1.0       bayesplot_1.8.0      shinythemes_1.2.0   
 [79] rstudioapi_0.13      gamm4_0.2-6          curl_4.3.1          
 [82] reprex_2.0.0         bslib_0.2.5.1        stringi_1.6.2       
 [85] ps_1.6.0             Brobdingnag_1.2-6    lattice_0.20-44     
 [88] Matrix_1.3-4         nloptr_1.2.2.2       markdown_1.1        
 [91] shinyjs_2.0.0        vctrs_0.3.8          pillar_1.6.1        
 [94] lifecycle_1.0.0      jquerylib_0.1.4      bridgesampling_1.1-2
 [97] estimability_1.3     httpuv_1.6.1         R6_2.5.0            
[100] promises_1.2.0.1     gridExtra_2.3        codetools_0.2-18    
[103] boot_1.3-28          colourpicker_1.1.0   MASS_7.3-54         
[106] gtools_3.9.2         assertthat_0.2.1     withr_2.4.2         
[109] shinystan_2.5.0      multcomp_1.4-17      mgcv_1.8-36         
[112] hms_1.1.0            grid_4.1.0           coda_0.19-4         
[115] minqa_1.2.4          rmarkdown_2.8        shiny_1.6.0         
[118] lubridate_1.7.10     base64enc_0.1-3      dygraphs_1.1.1.6    
```