Tables
=================================================
This report creates the tables.

<!--  Set the working directory to the repository's base directory; this assumes the report is nested inside of only one directory.-->

```r
library(knitr)
knitr::opts_knit$set(root.dir='../')  #Don't combine this call with any other chunk -especially one that uses file paths.
```

<!-- Set the report-wide options, and point to the external code file. -->

```r
report_render_start_time <- Sys.time()
opts_chunk$set(
  results = 'asis',
  message = TRUE,
  comment = NA,
  tidy = FALSE
)
echoChunks <- FALSE
options(width=80) # Default width
read_chunk("./tables/tables.R")
```
<!-- Load the packages.  Suppress the output when loading packages. -->


<!-- Load any Global functions and variables declared in the R file.  Suppress the output. -->


<!-- Declare any global functions specific to a Rmd output.  Suppress the output. -->


<!-- Load the datasets.   -->


<!-- Tweak the datasets.   -->


## Table A.1: Standard normal distribution

|Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |Z    |Inside |Outside |
|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|:----|:------|:-------|
|0.00 |.0000  |.5000   |0.38 |.1480  |.3520   |0.76 |.2764  |.2236   |1.14 |.3729  |.1271   |1.52 |.4357  |.0643   |1.90 |.4713  |.0287   |2.28 |.4887  |.0113   |2.66 |.4961  |.0039   |3.04 |.4988  |.0012   |
|0.01 |.0040  |.4960   |0.39 |.1517  |.3483   |0.77 |.2794  |.2206   |1.15 |.3749  |.1251   |1.53 |.4370  |.0630   |1.91 |.4719  |.0281   |2.29 |.4890  |.0110   |2.67 |.4962  |.0038   |3.05 |.4989  |.0011   |
|0.02 |.0080  |.4920   |0.40 |.1554  |.3446   |0.78 |.2823  |.2177   |1.16 |.3770  |.1230   |1.54 |.4382  |.0618   |1.92 |.4726  |.0274   |2.30 |.4893  |.0107   |2.68 |.4963  |.0037   |3.06 |.4989  |.0011   |
|0.03 |.0120  |.4880   |0.41 |.1591  |.3409   |0.79 |.2852  |.2148   |1.17 |.3790  |.1210   |1.55 |.4394  |.0606   |1.93 |.4732  |.0268   |2.31 |.4896  |.0104   |2.69 |.4964  |.0036   |3.07 |.4989  |.0011   |
|0.04 |.0160  |.4840   |0.42 |.1628  |.3372   |0.80 |.2881  |.2119   |1.18 |.3810  |.1190   |1.56 |.4406  |.0594   |1.94 |.4738  |.0262   |2.32 |.4898  |.0102   |2.70 |.4965  |.0035   |3.08 |.4990  |.0010   |
|0.05 |.0199  |.4801   |0.43 |.1664  |.3336   |0.81 |.2910  |.2090   |1.19 |.3830  |.1170   |1.57 |.4418  |.0582   |1.95 |.4744  |.0256   |2.33 |.4901  |.0099   |2.71 |.4966  |.0034   |3.09 |.4990  |.0010   |
|0.06 |.0239  |.4761   |0.44 |.1700  |.3300   |0.82 |.2939  |.2061   |1.20 |.3849  |.1151   |1.58 |.4429  |.0571   |1.96 |.4750  |.0250   |2.34 |.4904  |.0096   |2.72 |.4967  |.0033   |3.10 |.4990  |.0010   |
|0.07 |.0279  |.4721   |0.45 |.1736  |.3264   |0.83 |.2967  |.2033   |1.21 |.3869  |.1131   |1.59 |.4441  |.0559   |1.97 |.4756  |.0244   |2.35 |.4906  |.0094   |2.73 |.4968  |.0032   |3.11 |.4991  |.0009   |
|0.08 |.0319  |.4681   |0.46 |.1772  |.3228   |0.84 |.2995  |.2005   |1.22 |.3888  |.1112   |1.60 |.4452  |.0548   |1.98 |.4761  |.0239   |2.36 |.4909  |.0091   |2.74 |.4969  |.0031   |3.12 |.4991  |.0009   |
|0.09 |.0359  |.4641   |0.47 |.1808  |.3192   |0.85 |.3023  |.1977   |1.23 |.3907  |.1093   |1.61 |.4463  |.0537   |1.99 |.4767  |.0233   |2.37 |.4911  |.0089   |2.75 |.4970  |.0030   |3.13 |.4991  |.0009   |
|0.10 |.0398  |.4602   |0.48 |.1844  |.3156   |0.86 |.3051  |.1949   |1.24 |.3925  |.1075   |1.62 |.4474  |.0526   |2.00 |.4772  |.0228   |2.38 |.4913  |.0087   |2.76 |.4971  |.0029   |3.14 |.4992  |.0008   |
|0.11 |.0438  |.4562   |0.49 |.1879  |.3121   |0.87 |.3078  |.1922   |1.25 |.3944  |.1056   |1.63 |.4484  |.0516   |2.01 |.4778  |.0222   |2.39 |.4916  |.0084   |2.77 |.4972  |.0028   |3.15 |.4992  |.0008   |
|0.12 |.0478  |.4522   |0.50 |.1915  |.3085   |0.88 |.3106  |.1894   |1.26 |.3962  |.1038   |1.64 |.4495  |.0505   |2.02 |.4783  |.0217   |2.40 |.4918  |.0082   |2.78 |.4973  |.0027   |3.16 |.4992  |.0008   |
|0.13 |.0517  |.4483   |0.51 |.1950  |.3050   |0.89 |.3133  |.1867   |1.27 |.3980  |.1020   |1.65 |.4505  |.0495   |2.03 |.4788  |.0212   |2.41 |.4920  |.0080   |2.79 |.4974  |.0026   |3.17 |.4992  |.0008   |
|0.14 |.0557  |.4443   |0.52 |.1985  |.3015   |0.90 |.3159  |.1841   |1.28 |.3997  |.1003   |1.66 |.4515  |.0485   |2.04 |.4793  |.0207   |2.42 |.4922  |.0078   |2.80 |.4974  |.0026   |3.18 |.4993  |.0007   |
|0.15 |.0596  |.4404   |0.53 |.2019  |.2981   |0.91 |.3186  |.1814   |1.29 |.4015  |.0985   |1.67 |.4525  |.0475   |2.05 |.4798  |.0202   |2.43 |.4925  |.0075   |2.81 |.4975  |.0025   |3.19 |.4993  |.0007   |
|0.16 |.0636  |.4364   |0.54 |.2054  |.2946   |0.92 |.3212  |.1788   |1.30 |.4032  |.0968   |1.68 |.4535  |.0465   |2.06 |.4803  |.0197   |2.44 |.4927  |.0073   |2.82 |.4976  |.0024   |3.20 |.4993  |.0007   |
|0.17 |.0675  |.4325   |0.55 |.2088  |.2912   |0.93 |.3238  |.1762   |1.31 |.4049  |.0951   |1.69 |.4545  |.0455   |2.07 |.4808  |.0192   |2.45 |.4929  |.0071   |2.83 |.4977  |.0023   |3.21 |.4993  |.0007   |
|0.18 |.0714  |.4286   |0.56 |.2123  |.2877   |0.94 |.3264  |.1736   |1.32 |.4066  |.0934   |1.70 |.4554  |.0446   |2.08 |.4812  |.0188   |2.46 |.4931  |.0069   |2.84 |.4977  |.0023   |3.22 |.4994  |.0006   |
|0.19 |.0753  |.4247   |0.57 |.2157  |.2843   |0.95 |.3289  |.1711   |1.33 |.4082  |.0918   |1.71 |.4564  |.0436   |2.09 |.4817  |.0183   |2.47 |.4932  |.0068   |2.85 |.4978  |.0022   |3.23 |.4994  |.0006   |
|0.20 |.0793  |.4207   |0.58 |.2190  |.2810   |0.96 |.3315  |.1685   |1.34 |.4099  |.0901   |1.72 |.4573  |.0427   |2.10 |.4821  |.0179   |2.48 |.4934  |.0066   |2.86 |.4979  |.0021   |3.24 |.4994  |.0006   |
|0.21 |.0832  |.4168   |0.59 |.2224  |.2776   |0.97 |.3340  |.1660   |1.35 |.4115  |.0885   |1.73 |.4582  |.0418   |2.11 |.4826  |.0174   |2.49 |.4936  |.0064   |2.87 |.4979  |.0021   |3.25 |.4994  |.0006   |
|0.22 |.0871  |.4129   |0.60 |.2257  |.2743   |0.98 |.3365  |.1635   |1.36 |.4131  |.0869   |1.74 |.4591  |.0409   |2.12 |.4830  |.0170   |2.50 |.4938  |.0062   |2.88 |.4980  |.0020   |3.30 |.49952 |.00048  |
|0.23 |.0910  |.4090   |0.61 |.2291  |.2709   |0.99 |.3389  |.1611   |1.37 |.4147  |.0853   |1.75 |.4599  |.0401   |2.13 |.4834  |.0166   |2.51 |.4940  |.0060   |2.89 |.4981  |.0019   |3.35 |.49960 |.00040  |
|0.24 |.0948  |.4052   |0.62 |.2324  |.2676   |1.00 |.3413  |.1587   |1.38 |.4162  |.0838   |1.76 |.4608  |.0392   |2.14 |.4838  |.0162   |2.52 |.4941  |.0059   |2.90 |.4981  |.0019   |3.40 |.49966 |.00034  |
|0.25 |.0987  |.4013   |0.63 |.2357  |.2643   |1.01 |.3438  |.1562   |1.39 |.4177  |.0823   |1.77 |.4616  |.0384   |2.15 |.4842  |.0158   |2.53 |.4943  |.0057   |2.91 |.4982  |.0018   |3.45 |.49972 |.00028  |
|0.26 |.1026  |.3974   |0.64 |.2389  |.2611   |1.02 |.3461  |.1539   |1.40 |.4192  |.0808   |1.78 |.4625  |.0375   |2.16 |.4846  |.0154   |2.54 |.4945  |.0055   |2.92 |.4982  |.0018   |3.50 |.49977 |.00023  |
|0.27 |.1064  |.3936   |0.65 |.2422  |.2578   |1.03 |.3485  |.1515   |1.41 |.4207  |.0793   |1.79 |.4633  |.0367   |2.17 |.4850  |.0150   |2.55 |.4946  |.0054   |2.93 |.4983  |.0017   |3.60 |.49984 |.00016  |
|0.28 |.1103  |.3897   |0.66 |.2454  |.2546   |1.04 |.3508  |.1492   |1.42 |.4222  |.0778   |1.80 |.4641  |.0359   |2.18 |.4854  |.0146   |2.56 |.4948  |.0052   |2.94 |.4984  |.0016   |3.70 |.49989 |.00011  |
|0.29 |.1141  |.3859   |0.67 |.2486  |.2514   |1.05 |.3531  |.1469   |1.43 |.4236  |.0764   |1.81 |.4649  |.0351   |2.19 |.4857  |.0143   |2.57 |.4949  |.0051   |2.95 |.4984  |.0016   |3.80 |.49993 |.00007  |
|0.30 |.1179  |.3821   |0.68 |.2517  |.2483   |1.06 |.3554  |.1446   |1.44 |.4251  |.0749   |1.82 |.4656  |.0344   |2.20 |.4861  |.0139   |2.58 |.4951  |.0049   |2.96 |.4985  |.0015   |3.90 |.49995 |.00005  |
|0.31 |.1217  |.3783   |0.69 |.2549  |.2451   |1.07 |.3577  |.1423   |1.45 |.4265  |.0735   |1.83 |.4664  |.0336   |2.21 |.4864  |.0136   |2.59 |.4952  |.0048   |2.97 |.4985  |.0015   |4.00 |.49997 |.00003  |
|0.32 |.1255  |.3745   |0.70 |.2580  |.2420   |1.08 |.3599  |.1401   |1.46 |.4279  |.0721   |1.84 |.4671  |.0329   |2.22 |.4868  |.0132   |2.60 |.4953  |.0047   |2.98 |.4986  |.0014   |     |       |        |
|0.33 |.1293  |.3707   |0.71 |.2611  |.2389   |1.09 |.3621  |.1379   |1.47 |.4292  |.0708   |1.85 |.4678  |.0322   |2.23 |.4871  |.0129   |2.61 |.4955  |.0045   |2.99 |.4986  |.0014   |     |       |        |
|0.34 |.1331  |.3669   |0.72 |.2642  |.2358   |1.10 |.3643  |.1357   |1.48 |.4306  |.0694   |1.86 |.4686  |.0314   |2.24 |.4875  |.0125   |2.62 |.4956  |.0044   |3.00 |.4987  |.0013   |     |       |        |
|0.35 |.1368  |.3632   |0.73 |.2673  |.2327   |1.11 |.3665  |.1335   |1.49 |.4319  |.0681   |1.87 |.4693  |.0307   |2.25 |.4878  |.0122   |2.63 |.4957  |.0043   |3.01 |.4987  |.0013   |     |       |        |
|0.36 |.1406  |.3594   |0.74 |.2704  |.2296   |1.12 |.3686  |.1314   |1.50 |.4332  |.0668   |1.88 |.4699  |.0301   |2.26 |.4881  |.0119   |2.64 |.4959  |.0041   |3.02 |.4987  |.0013   |     |       |        |
|0.37 |.1443  |.3557   |0.75 |.2734  |.2266   |1.13 |.3708  |.1292   |1.51 |.4345  |.0655   |1.89 |.4706  |.0294   |2.27 |.4884  |.0116   |2.65 |.4960  |.0040   |3.03 |.4988  |.0012   |     |       |        |

## Table B.1: Critical values for *t* distributions

|     df| Alpha10| Alpha05| Alpha025| Alpha01| Alpha005| Alpha0005|
|------:|-------:|-------:|--------:|-------:|--------:|---------:|
|      1|   3.078|   6.314|   12.706|  31.821|   63.657|   636.619|
|      2|   1.886|   2.920|    4.303|   6.965|    9.925|    31.599|
|      3|   1.638|   2.353|    3.182|   4.541|    5.841|    12.924|
|      4|   1.533|   2.132|    2.776|   3.747|    4.604|     8.610|
|      5|   1.476|   2.015|    2.571|   3.365|    4.032|     6.869|
|      6|   1.440|   1.943|    2.447|   3.143|    3.707|     5.959|
|      7|   1.415|   1.895|    2.365|   2.998|    3.499|     5.408|
|      8|   1.397|   1.860|    2.306|   2.896|    3.355|     5.041|
|      9|   1.383|   1.833|    2.262|   2.821|    3.250|     4.781|
|     10|   1.372|   1.812|    2.228|   2.764|    3.169|     4.587|
|     11|   1.363|   1.796|    2.201|   2.718|    3.106|     4.437|
|     12|   1.356|   1.782|    2.179|   2.681|    3.055|     4.318|
|     13|   1.350|   1.771|    2.160|   2.650|    3.012|     4.221|
|     14|   1.345|   1.761|    2.145|   2.624|    2.977|     4.140|
|     15|   1.341|   1.753|    2.131|   2.602|    2.947|     4.073|
|     16|   1.337|   1.746|    2.120|   2.583|    2.921|     4.015|
|     17|   1.333|   1.740|    2.110|   2.567|    2.898|     3.965|
|     18|   1.330|   1.734|    2.101|   2.552|    2.878|     3.922|
|     19|   1.328|   1.729|    2.093|   2.539|    2.861|     3.883|
|     20|   1.325|   1.725|    2.086|   2.528|    2.845|     3.850|
|     21|   1.323|   1.721|    2.080|   2.518|    2.831|     3.819|
|     22|   1.321|   1.717|    2.074|   2.508|    2.819|     3.792|
|     23|   1.319|   1.714|    2.069|   2.500|    2.807|     3.768|
|     24|   1.318|   1.711|    2.064|   2.492|    2.797|     3.745|
|     25|   1.316|   1.708|    2.060|   2.485|    2.787|     3.725|
|     26|   1.315|   1.706|    2.056|   2.479|    2.779|     3.707|
|     27|   1.314|   1.703|    2.052|   2.473|    2.771|     3.690|
|     28|   1.313|   1.701|    2.048|   2.467|    2.763|     3.674|
|     29|   1.311|   1.699|    2.045|   2.462|    2.756|     3.659|
|     30|   1.310|   1.697|    2.042|   2.457|    2.750|     3.646|
|     35|   1.306|   1.690|    2.030|   2.438|    2.724|     3.591|
|     40|   1.303|   1.684|    2.021|   2.423|    2.704|     3.551|
|     45|   1.301|   1.679|    2.014|   2.412|    2.690|     3.520|
|     50|   1.299|   1.676|    2.009|   2.403|    2.678|     3.496|
|     55|   1.297|   1.673|    2.004|   2.396|    2.668|     3.476|
|     60|   1.296|   1.671|    2.000|   2.390|    2.660|     3.460|
|     70|   1.294|   1.667|    1.994|   2.381|    2.648|     3.435|
|     80|   1.292|   1.664|    1.990|   2.374|    2.639|     3.416|
|     90|   1.291|   1.662|    1.987|   2.368|    2.632|     3.402|
|    120|   1.289|   1.658|    1.980|   2.358|    2.617|     3.373|
| 100000|   1.282|   1.645|    1.960|   2.326|    2.576|     3.291|

## Table C.1: Critical values for *F* distributions

| DenominatorDF| Alpha|     1|     2|     3|     4|     5|     6|     7|     8|     9|    10|    11|    12|    14|    16|    20|
|-------------:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|
|             1|  0.05|   161|   199|   216|   225|   230|   234|   237|   239|   241|   242|   243|   244|   245|   246|   248|
|             1|  0.01|  4052|  4999|  5403|  5625|  5764|  5859|  5928|  5981|  6022|  6056|  6083|  6106|  6143|  6170|  6209|
|             2|  0.05| 18.51| 19.00| 19.16| 19.25| 19.30| 19.33| 19.35| 19.37| 19.38| 19.40| 19.40| 19.41| 19.42| 19.43| 19.45|
|             2|  0.01| 98.50| 99.00| 99.17| 99.25| 99.30| 99.33| 99.36| 99.37| 99.39| 99.40| 99.41| 99.42| 99.43| 99.44| 99.45|
|             3|  0.05| 10.13|  9.55|  9.28|  9.12|  9.01|  8.94|  8.89|  8.85|  8.81|  8.79|  8.76|  8.74|  8.71|  8.69|  8.66|
|             3|  0.01| 34.12| 30.82| 29.46| 28.71| 28.24| 27.91| 27.67| 27.49| 27.35| 27.23| 27.13| 27.05| 26.92| 26.83| 26.69|
|             4|  0.05|  7.71|  6.94|  6.59|  6.39|  6.26|  6.16|  6.09|  6.04|  6.00|  5.96|  5.94|  5.91|  5.87|  5.84|  5.80|
|             4|  0.01| 21.20| 18.00| 16.69| 15.98| 15.52| 15.21| 14.98| 14.80| 14.66| 14.55| 14.45| 14.37| 14.25| 14.15| 14.02|
|             5|  0.05|  6.61|  5.79|  5.41|  5.19|  5.05|  4.95|  4.88|  4.82|  4.77|  4.74|  4.70|  4.68|  4.64|  4.60|  4.56|
|             5|  0.01| 16.26| 13.27| 12.06| 11.39| 10.97| 10.67| 10.46| 10.29| 10.16| 10.05|  9.96|  9.89|  9.77|  9.68|  9.55|
|             6|  0.05|  5.99|  5.14|  4.76|  4.53|  4.39|  4.28|  4.21|  4.15|  4.10|  4.06|  4.03|  4.00|  3.96|  3.92|  3.87|
|             6|  0.01| 13.75| 10.92|  9.78|  9.15|  8.75|  8.47|  8.26|  8.10|  7.98|  7.87|  7.79|  7.72|  7.60|  7.52|  7.40|
|             7|  0.05|  5.59|  4.74|  4.35|  4.12|  3.97|  3.87|  3.79|  3.73|  3.68|  3.64|  3.60|  3.57|  3.53|  3.49|  3.44|
|             7|  0.01| 12.25|  9.55|  8.45|  7.85|  7.46|  7.19|  6.99|  6.84|  6.72|  6.62|  6.54|  6.47|  6.36|  6.28|  6.16|
|             8|  0.05|  5.32|  4.46|  4.07|  3.84|  3.69|  3.58|  3.50|  3.44|  3.39|  3.35|  3.31|  3.28|  3.24|  3.20|  3.15|
|             8|  0.01| 11.26|  8.65|  7.59|  7.01|  6.63|  6.37|  6.18|  6.03|  5.91|  5.81|  5.73|  5.67|  5.56|  5.48|  5.36|
|             9|  0.05|  5.12|  4.26|  3.86|  3.63|  3.48|  3.37|  3.29|  3.23|  3.18|  3.14|  3.10|  3.07|  3.03|  2.99|  2.94|
|             9|  0.01| 10.56|  8.02|  6.99|  6.42|  6.06|  5.80|  5.61|  5.47|  5.35|  5.26|  5.18|  5.11|  5.01|  4.92|  4.81|
|            10|  0.05|  4.96|  4.10|  3.71|  3.48|  3.33|  3.22|  3.14|  3.07|  3.02|  2.98|  2.94|  2.91|  2.86|  2.83|  2.77|
|            10|  0.01| 10.04|  7.56|  6.55|  5.99|  5.64|  5.39|  5.20|  5.06|  4.94|  4.85|  4.77|  4.71|  4.60|  4.52|  4.41|
|            11|  0.05|  4.84|  3.98|  3.59|  3.36|  3.20|  3.09|  3.01|  2.95|  2.90|  2.85|  2.82|  2.79|  2.74|  2.70|  2.65|
|            11|  0.01|  9.65|  7.21|  6.22|  5.67|  5.32|  5.07|  4.89|  4.74|  4.63|  4.54|  4.46|  4.40|  4.29|  4.21|  4.10|
|            12|  0.05|  4.75|  3.89|  3.49|  3.26|  3.11|  3.00|  2.91|  2.85|  2.80|  2.75|  2.72|  2.69|  2.64|  2.60|  2.54|
|            12|  0.01|  9.33|  6.93|  5.95|  5.41|  5.06|  4.82|  4.64|  4.50|  4.39|  4.30|  4.22|  4.16|  4.05|  3.97|  3.86|
|            13|  0.05|  4.67|  3.81|  3.41|  3.18|  3.03|  2.92|  2.83|  2.77|  2.71|  2.67|  2.63|  2.60|  2.55|  2.51|  2.46|
|            13|  0.01|  9.07|  6.70|  5.74|  5.21|  4.86|  4.62|  4.44|  4.30|  4.19|  4.10|  4.02|  3.96|  3.86|  3.78|  3.66|
|            14|  0.05|  4.60|  3.74|  3.34|  3.11|  2.96|  2.85|  2.76|  2.70|  2.65|  2.60|  2.57|  2.53|  2.48|  2.44|  2.39|
|            14|  0.01|  8.86|  6.51|  5.56|  5.04|  4.69|  4.46|  4.28|  4.14|  4.03|  3.94|  3.86|  3.80|  3.70|  3.62|  3.51|
|            15|  0.05|  4.54|  3.68|  3.29|  3.06|  2.90|  2.79|  2.71|  2.64|  2.59|  2.54|  2.51|  2.48|  2.42|  2.38|  2.33|
|            15|  0.01|  8.68|  6.36|  5.42|  4.89|  4.56|  4.32|  4.14|  4.00|  3.89|  3.80|  3.73|  3.67|  3.56|  3.49|  3.37|
|            16|  0.05|  4.49|  3.63|  3.24|  3.01|  2.85|  2.74|  2.66|  2.59|  2.54|  2.49|  2.46|  2.42|  2.37|  2.33|  2.28|
|            16|  0.01|  8.53|  6.23|  5.29|  4.77|  4.44|  4.20|  4.03|  3.89|  3.78|  3.69|  3.62|  3.55|  3.45|  3.37|  3.26|
|            17|  0.05|  4.45|  3.59|  3.20|  2.96|  2.81|  2.70|  2.61|  2.55|  2.49|  2.45|  2.41|  2.38|  2.33|  2.29|  2.23|
|            17|  0.01|  8.40|  6.11|  5.18|  4.67|  4.34|  4.10|  3.93|  3.79|  3.68|  3.59|  3.52|  3.46|  3.35|  3.27|  3.16|
|            18|  0.05|  4.41|  3.55|  3.16|  2.93|  2.77|  2.66|  2.58|  2.51|  2.46|  2.41|  2.37|  2.34|  2.29|  2.25|  2.19|
|            18|  0.01|  8.29|  6.01|  5.09|  4.58|  4.25|  4.01|  3.84|  3.71|  3.60|  3.51|  3.43|  3.37|  3.27|  3.19|  3.08|
|            19|  0.05|  4.38|  3.52|  3.13|  2.90|  2.74|  2.63|  2.54|  2.48|  2.42|  2.38|  2.34|  2.31|  2.26|  2.21|  2.16|
|            19|  0.01|  8.18|  5.93|  5.01|  4.50|  4.17|  3.94|  3.77|  3.63|  3.52|  3.43|  3.36|  3.30|  3.19|  3.12|  3.00|
|            20|  0.05|  4.35|  3.49|  3.10|  2.87|  2.71|  2.60|  2.51|  2.45|  2.39|  2.35|  2.31|  2.28|  2.22|  2.18|  2.12|
|            20|  0.01|  8.10|  5.85|  4.94|  4.43|  4.10|  3.87|  3.70|  3.56|  3.46|  3.37|  3.29|  3.23|  3.13|  3.05|  2.94|
|            21|  0.05|  4.32|  3.47|  3.07|  2.84|  2.68|  2.57|  2.49|  2.42|  2.37|  2.32|  2.28|  2.25|  2.20|  2.16|  2.10|
|            21|  0.01|  8.02|  5.78|  4.87|  4.37|  4.04|  3.81|  3.64|  3.51|  3.40|  3.31|  3.24|  3.17|  3.07|  2.99|  2.88|
|            22|  0.05|  4.30|  3.44|  3.05|  2.82|  2.66|  2.55|  2.46|  2.40|  2.34|  2.30|  2.26|  2.23|  2.17|  2.13|  2.07|
|            22|  0.01|  7.95|  5.72|  4.82|  4.31|  3.99|  3.76|  3.59|  3.45|  3.35|  3.26|  3.18|  3.12|  3.02|  2.94|  2.83|
|            23|  0.05|  4.28|  3.42|  3.03|  2.80|  2.64|  2.53|  2.44|  2.37|  2.32|  2.27|  2.24|  2.20|  2.15|  2.11|  2.05|
|            23|  0.01|  7.88|  5.66|  4.76|  4.26|  3.94|  3.71|  3.54|  3.41|  3.30|  3.21|  3.14|  3.07|  2.97|  2.89|  2.78|
|            24|  0.05|  4.26|  3.40|  3.01|  2.78|  2.62|  2.51|  2.42|  2.36|  2.30|  2.25|  2.22|  2.18|  2.13|  2.09|  2.03|
|            24|  0.01|  7.82|  5.61|  4.72|  4.22|  3.90|  3.67|  3.50|  3.36|  3.26|  3.17|  3.09|  3.03|  2.93|  2.85|  2.74|
|            25|  0.05|  4.24|  3.39|  2.99|  2.76|  2.60|  2.49|  2.40|  2.34|  2.28|  2.24|  2.20|  2.16|  2.11|  2.07|  2.01|
|            25|  0.01|  7.77|  5.57|  4.68|  4.18|  3.85|  3.63|  3.46|  3.32|  3.22|  3.13|  3.06|  2.99|  2.89|  2.81|  2.70|
|            26|  0.05|  4.23|  3.37|  2.98|  2.74|  2.59|  2.47|  2.39|  2.32|  2.27|  2.22|  2.18|  2.15|  2.09|  2.05|  1.99|
|            26|  0.01|  7.72|  5.53|  4.64|  4.14|  3.82|  3.59|  3.42|  3.29|  3.18|  3.09|  3.02|  2.96|  2.86|  2.78|  2.66|
|            27|  0.05|  4.21|  3.35|  2.96|  2.73|  2.57|  2.46|  2.37|  2.31|  2.25|  2.20|  2.17|  2.13|  2.08|  2.04|  1.97|
|            27|  0.01|  7.68|  5.49|  4.60|  4.11|  3.78|  3.56|  3.39|  3.26|  3.15|  3.06|  2.99|  2.93|  2.82|  2.75|  2.63|
|            28|  0.05|  4.20|  3.34|  2.95|  2.71|  2.56|  2.45|  2.36|  2.29|  2.24|  2.19|  2.15|  2.12|  2.06|  2.02|  1.96|
|            28|  0.01|  7.64|  5.45|  4.57|  4.07|  3.75|  3.53|  3.36|  3.23|  3.12|  3.03|  2.96|  2.90|  2.79|  2.72|  2.60|
|            29|  0.05|  4.18|  3.33|  2.93|  2.70|  2.55|  2.43|  2.35|  2.28|  2.22|  2.18|  2.14|  2.10|  2.05|  2.01|  1.94|
|            29|  0.01|  7.60|  5.42|  4.54|  4.04|  3.73|  3.50|  3.33|  3.20|  3.09|  3.00|  2.93|  2.87|  2.77|  2.69|  2.57|
|            30|  0.05|  4.17|  3.32|  2.92|  2.69|  2.53|  2.42|  2.33|  2.27|  2.21|  2.16|  2.13|  2.09|  2.04|  1.99|  1.93|
|            30|  0.01|  7.56|  5.39|  4.51|  4.02|  3.70|  3.47|  3.30|  3.17|  3.07|  2.98|  2.91|  2.84|  2.74|  2.66|  2.55|
|            32|  0.05|  4.15|  3.29|  2.90|  2.67|  2.51|  2.40|  2.31|  2.24|  2.19|  2.14|  2.10|  2.07|  2.01|  1.97|  1.91|
|            32|  0.01|  7.50|  5.34|  4.46|  3.97|  3.65|  3.43|  3.26|  3.13|  3.02|  2.93|  2.86|  2.80|  2.70|  2.62|  2.50|
|            34|  0.05|  4.13|  3.28|  2.88|  2.65|  2.49|  2.38|  2.29|  2.23|  2.17|  2.12|  2.08|  2.05|  1.99|  1.95|  1.89|
|            34|  0.01|  7.44|  5.29|  4.42|  3.93|  3.61|  3.39|  3.22|  3.09|  2.98|  2.89|  2.82|  2.76|  2.66|  2.58|  2.46|
|            36|  0.05|  4.11|  3.26|  2.87|  2.63|  2.48|  2.36|  2.28|  2.21|  2.15|  2.11|  2.07|  2.03|  1.98|  1.93|  1.87|
|            36|  0.01|  7.40|  5.25|  4.38|  3.89|  3.57|  3.35|  3.18|  3.05|  2.95|  2.86|  2.79|  2.72|  2.62|  2.54|  2.43|
|            38|  0.05|  4.10|  3.24|  2.85|  2.62|  2.46|  2.35|  2.26|  2.19|  2.14|  2.09|  2.05|  2.02|  1.96|  1.92|  1.85|
|            38|  0.01|  7.35|  5.21|  4.34|  3.86|  3.54|  3.32|  3.15|  3.02|  2.92|  2.83|  2.75|  2.69|  2.59|  2.51|  2.40|
|            40|  0.05|  4.08|  3.23|  2.84|  2.61|  2.45|  2.34|  2.25|  2.18|  2.12|  2.08|  2.04|  2.00|  1.95|  1.90|  1.84|
|            40|  0.01|  7.31|  5.18|  4.31|  3.83|  3.51|  3.29|  3.12|  2.99|  2.89|  2.80|  2.73|  2.66|  2.56|  2.48|  2.37|
|            42|  0.05|  4.07|  3.22|  2.83|  2.59|  2.44|  2.32|  2.24|  2.17|  2.11|  2.06|  2.03|  1.99|  1.94|  1.89|  1.83|
|            42|  0.01|  7.28|  5.15|  4.29|  3.80|  3.49|  3.27|  3.10|  2.97|  2.86|  2.78|  2.70|  2.64|  2.54|  2.46|  2.34|
|            44|  0.05|  4.06|  3.21|  2.82|  2.58|  2.43|  2.31|  2.23|  2.16|  2.10|  2.05|  2.01|  1.98|  1.92|  1.88|  1.81|
|            44|  0.01|  7.25|  5.12|  4.26|  3.78|  3.47|  3.24|  3.08|  2.95|  2.84|  2.75|  2.68|  2.62|  2.52|  2.44|  2.32|
|            46|  0.05|  4.05|  3.20|  2.81|  2.57|  2.42|  2.30|  2.22|  2.15|  2.09|  2.04|  2.00|  1.97|  1.91|  1.87|  1.80|
|            46|  0.01|  7.22|  5.10|  4.24|  3.76|  3.44|  3.22|  3.06|  2.93|  2.82|  2.73|  2.66|  2.60|  2.50|  2.42|  2.30|
|            48|  0.05|  4.04|  3.19|  2.80|  2.57|  2.41|  2.29|  2.21|  2.14|  2.08|  2.03|  1.99|  1.96|  1.90|  1.86|  1.79|
|            48|  0.01|  7.19|  5.08|  4.22|  3.74|  3.43|  3.20|  3.04|  2.91|  2.80|  2.71|  2.64|  2.58|  2.48|  2.40|  2.28|
|            50|  0.05|  4.03|  3.18|  2.79|  2.56|  2.40|  2.29|  2.20|  2.13|  2.07|  2.03|  1.99|  1.95|  1.89|  1.85|  1.78|
|            50|  0.01|  7.17|  5.06|  4.20|  3.72|  3.41|  3.19|  3.02|  2.89|  2.78|  2.70|  2.63|  2.56|  2.46|  2.38|  2.27|
|            55|  0.05|  4.02|  3.16|  2.77|  2.54|  2.38|  2.27|  2.18|  2.11|  2.06|  2.01|  1.97|  1.93|  1.88|  1.83|  1.76|
|            55|  0.01|  7.12|  5.01|  4.16|  3.68|  3.37|  3.15|  2.98|  2.85|  2.75|  2.66|  2.59|  2.53|  2.42|  2.34|  2.23|
|            60|  0.05|  4.00|  3.15|  2.76|  2.53|  2.37|  2.25|  2.17|  2.10|  2.04|  1.99|  1.95|  1.92|  1.86|  1.82|  1.75|
|            60|  0.01|  7.08|  4.98|  4.13|  3.65|  3.34|  3.12|  2.95|  2.82|  2.72|  2.63|  2.56|  2.50|  2.39|  2.31|  2.20|
|            70|  0.05|  3.98|  3.13|  2.74|  2.50|  2.35|  2.23|  2.14|  2.07|  2.02|  1.97|  1.93|  1.89|  1.84|  1.79|  1.72|
|            70|  0.01|  7.01|  4.92|  4.07|  3.60|  3.29|  3.07|  2.91|  2.78|  2.67|  2.59|  2.51|  2.45|  2.35|  2.27|  2.15|
|            80|  0.05|  3.96|  3.11|  2.72|  2.49|  2.33|  2.21|  2.13|  2.06|  2.00|  1.95|  1.91|  1.88|  1.82|  1.77|  1.70|
|            80|  0.01|  6.96|  4.88|  4.04|  3.56|  3.26|  3.04|  2.87|  2.74|  2.64|  2.55|  2.48|  2.42|  2.31|  2.23|  2.12|
|           100|  0.05|  3.94|  3.09|  2.70|  2.46|  2.31|  2.19|  2.10|  2.03|  1.97|  1.93|  1.89|  1.85|  1.79|  1.75|  1.68|
|           100|  0.01|  6.90|  4.82|  3.98|  3.51|  3.21|  2.99|  2.82|  2.69|  2.59|  2.50|  2.43|  2.37|  2.27|  2.19|  2.07|
|           125|  0.05|  3.92|  3.07|  2.68|  2.44|  2.29|  2.17|  2.08|  2.01|  1.96|  1.91|  1.87|  1.83|  1.77|  1.73|  1.66|
|           125|  0.01|  6.84|  4.78|  3.94|  3.47|  3.17|  2.95|  2.79|  2.66|  2.55|  2.47|  2.39|  2.33|  2.23|  2.15|  2.03|
|           150|  0.05|  3.90|  3.06|  2.66|  2.43|  2.27|  2.16|  2.07|  2.00|  1.94|  1.89|  1.85|  1.82|  1.76|  1.71|  1.64|
|           150|  0.01|  6.81|  4.75|  3.91|  3.45|  3.14|  2.92|  2.76|  2.63|  2.53|  2.44|  2.37|  2.31|  2.20|  2.12|  2.00|
|           200|  0.05|  3.89|  3.04|  2.65|  2.42|  2.26|  2.14|  2.06|  1.98|  1.93|  1.88|  1.84|  1.80|  1.74|  1.69|  1.62|
|           200|  0.01|  6.76|  4.71|  3.88|  3.41|  3.11|  2.89|  2.73|  2.60|  2.50|  2.41|  2.34|  2.27|  2.17|  2.09|  1.97|
|           400|  0.05|  3.86|  3.02|  2.63|  2.39|  2.24|  2.12|  2.03|  1.96|  1.90|  1.85|  1.81|  1.78|  1.72|  1.67|  1.60|
|           400|  0.01|  6.70|  4.66|  3.83|  3.37|  3.06|  2.85|  2.68|  2.56|  2.45|  2.37|  2.29|  2.23|  2.13|  2.05|  1.92|
|          1000|  0.05|  3.85|  3.00|  2.61|  2.38|  2.22|  2.11|  2.02|  1.95|  1.89|  1.84|  1.80|  1.76|  1.70|  1.65|  1.58|
|          1000|  0.01|  6.66|  4.63|  3.80|  3.34|  3.04|  2.82|  2.66|  2.53|  2.43|  2.34|  2.27|  2.20|  2.10|  2.02|  1.90|
|      10000000|  0.05|  3.84|  3.00|  2.60|  2.37|  2.21|  2.10|  2.01|  1.94|  1.88|  1.83|  1.79|  1.75|  1.69|  1.64|  1.57|
|      10000000|  0.01|  6.63|  4.61|  3.78|  3.32|  3.02|  2.80|  2.64|  2.51|  2.41|  2.32|  2.25|  2.18|  2.08|  2.00|  1.88|

## Table D.1: Critical values for χ^2 distributions

| df| Alpha10| Alpha05| Alpha01| Alpha001|
|--:|-------:|-------:|-------:|--------:|
|  1|    2.71|    3.84|    6.63|    10.83|
|  2|    4.61|    5.99|    9.21|    13.82|
|  3|    6.25|    7.81|   11.34|    16.27|
|  4|    7.78|    9.49|   13.28|    18.47|
|  5|    9.24|   11.07|   15.09|    20.52|
|  6|   10.64|   12.59|   16.81|    22.46|
|  7|   12.02|   14.07|   18.48|    24.32|
|  8|   13.36|   15.51|   20.09|    26.12|
|  9|   14.68|   16.92|   21.67|    27.88|
| 10|   15.99|   18.31|   23.21|    29.59|
| 11|   17.28|   19.68|   24.72|    31.26|
| 12|   18.55|   21.03|   26.22|    32.91|
| 13|   19.81|   22.36|   27.69|    34.53|
| 14|   21.06|   23.68|   29.14|    36.12|
| 15|   22.31|   25.00|   30.58|    37.70|
| 16|   23.54|   26.30|   32.00|    39.25|
| 17|   24.77|   27.59|   33.41|    40.79|
| 18|   25.99|   28.87|   34.81|    42.31|
| 19|   27.20|   30.14|   36.19|    43.82|
| 20|   28.41|   31.41|   37.57|    45.31|
| 21|   29.62|   32.67|   38.93|    46.80|
| 22|   30.81|   33.92|   40.29|    48.27|
| 23|   32.01|   35.17|   41.64|    49.73|
| 24|   33.20|   36.42|   42.98|    51.18|
| 25|   34.38|   37.65|   44.31|    52.62|
| 26|   35.56|   38.89|   45.64|    54.05|
| 27|   36.74|   40.11|   46.96|    55.48|
| 28|   37.92|   41.34|   48.28|    56.89|
| 29|   39.09|   42.56|   49.59|    58.30|
| 30|   40.26|   43.77|   50.89|    59.70|
| 40|   51.81|   55.76|   63.69|    73.40|
| 50|   63.17|   67.50|   76.15|    86.66|
| 60|   74.40|   79.08|   88.38|    99.61|
| 70|   85.53|   90.53|  100.43|   112.32|

<!-- The footer that's common to all reports. -->

## Session Information

For the sake of documentation and reproducibility, the current report was rendered in the following environment.  Click the line below to expand.

<details>
  <summary>Environment <span class="glyphicon glyphicon-plus-sign"></span></summary>

```
Session info -------------------------------------------------------------------
```

```
 setting  value                       
 version  R version 3.3.3 (2017-03-06)
 system   x86_64, linux-gnu           
 ui       RStudio (1.0.136)           
 language en_US                       
 collate  en_US.UTF-8                 
 tz       America/Chicago             
 date     2017-04-02                  
```

```
Packages -----------------------------------------------------------------------
```

```
 package      * version    date       source                            
 assertthat     0.1        2013-12-06 CRAN (R 3.3.0)                    
 backports      1.0.5      2017-01-18 CRAN (R 3.3.1)                    
 colorspace     1.3-2      2016-12-14 CRAN (R 3.3.1)                    
 DBI            0.6        2017-03-09 CRAN (R 3.3.1)                    
 devtools       1.12.0     2016-06-24 CRAN (R 3.3.1)                    
 dichromat      2.0-0      2013-01-24 CRAN (R 3.3.0)                    
 digest         0.6.12     2017-01-27 CRAN (R 3.3.1)                    
 dplyr          0.5.0      2016-06-24 CRAN (R 3.3.3)                    
 epade          0.3.8      2013-02-22 CRAN (R 3.3.3)                    
 evaluate       0.10       2016-10-11 CRAN (R 3.3.1)                    
 extrafont      0.17       2014-12-08 CRAN (R 3.3.0)                    
 extrafontdb    1.0        2012-06-11 CRAN (R 3.3.0)                    
 ggplot2      * 2.2.1      2016-12-30 CRAN (R 3.3.1)                    
 gridExtra      2.2.1      2016-02-29 CRAN (R 3.3.0)                    
 gtable         0.2.0      2016-02-26 CRAN (R 3.3.0)                    
 highr          0.6        2016-05-09 CRAN (R 3.3.0)                    
 hms            0.3        2016-11-22 CRAN (R 3.3.1)                    
 htmltools      0.3.5      2016-03-21 CRAN (R 3.3.0)                    
 htmlwidgets    0.8        2016-11-09 CRAN (R 3.3.1)                    
 httpuv         1.3.3      2015-08-04 CRAN (R 3.3.0)                    
 jsonlite       1.3        2017-02-28 CRAN (R 3.3.1)                    
 knitr        * 1.15.1     2016-11-22 CRAN (R 3.3.1)                    
 labeling       0.3        2014-08-23 CRAN (R 3.3.0)                    
 lazyeval       0.2.0      2016-06-12 CRAN (R 3.3.0)                    
 magrittr     * 1.5        2014-11-22 CRAN (R 3.3.0)                    
 memoise        1.0.0      2016-01-29 CRAN (R 3.3.0)                    
 mime           0.5        2016-07-07 CRAN (R 3.3.1)                    
 munsell        0.4.3      2016-02-13 CRAN (R 3.3.0)                    
 pacman         0.4.1      2016-03-30 CRAN (R 3.3.3)                    
 plotrix        3.6-4      2016-12-30 CRAN (R 3.3.3)                    
 plyr           1.8.4      2016-06-08 CRAN (R 3.3.0)                    
 R6             2.2.0      2016-10-05 CRAN (R 3.3.1)                    
 RColorBrewer   1.1-2      2014-12-07 CRAN (R 3.3.0)                    
 Rcpp           0.12.10    2017-03-19 CRAN (R 3.3.1)                    
 readr          1.1.0      2017-03-22 CRAN (R 3.3.3)                    
 reshape2       1.4.2      2016-10-22 CRAN (R 3.3.1)                    
 rgl            0.98.1     2017-03-08 CRAN (R 3.3.1)                    
 rmarkdown      1.4.0.9000 2017-04-01 Github (rstudio/rmarkdown@5f7cd3c)
 rprojroot      1.2        2017-01-16 CRAN (R 3.3.1)                    
 rstudioapi     0.6        2016-06-27 CRAN (R 3.3.1)                    
 Rttf2pt1       1.3.4      2016-05-19 CRAN (R 3.3.0)                    
 scales         0.4.1      2016-11-09 CRAN (R 3.3.1)                    
 shiny          1.0.1      2017-04-01 CRAN (R 3.3.3)                    
 stringi        1.1.3      2017-03-21 CRAN (R 3.3.1)                    
 stringr        1.2.0      2017-02-18 CRAN (R 3.3.1)                    
 tibble         1.3.0      2017-04-01 CRAN (R 3.3.3)                    
 tidyr          0.6.1      2017-01-10 CRAN (R 3.3.1)                    
 wesanderson    0.3.2      2015-01-22 CRAN (R 3.3.3)                    
 withr          1.0.2      2016-06-20 CRAN (R 3.3.0)                    
 xtable         1.8-2      2016-02-05 CRAN (R 3.3.0)                    
 yaml           2.1.14     2016-11-12 CRAN (R 3.3.1)                    
```
</details>



Report rendered by wibeasley at 2017-04-02, 16:49 -0500 in 1 seconds.


## License

<a rel="license" href="http://creativecommons.org/licenses/by/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by/3.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/3.0/">Creative Commons Attribution 3.0 Unported License</a>.
