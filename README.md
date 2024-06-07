# QTXNetwork_3.0

## Getting Started
Check [QTXNetwork3.0 wiki](https://github.com/Zhutn/QTXNetwork3.0/wiki) for kicking off.
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Run with example data

**Options for QTXNetwork3.0**

* `--map` genetic map for QTL or genotype for QTS.

* `--txt` txt for QTL or phenotype for QTS.

* `--QTX` 0 for QTL mapping or 1 for QTS (default, QTL).

* `--threads` thread number (default, maximum).

* `--test-window` The size of testing window for background control. (default, 10.0 cM).

* `--scan-step` The genetic distance of step for QTL mapping. (default, 1.0 cM).

* `--only-1D` 1D scan only (--only-1D "any integer"). (default, False).

* `--output-1D` Output the results of HendersonIII F values for 1D scan (--output-1D "any integer"). (default, False).

**Choose a suitable version to conduct the analysis**
Using the CPU parallel version
```
cd CPU
```
Using the GPU parallel version
```
cd GPU
```

**Examples forQTXNetwork3.0**

```
./QTXNetwork --map ../example/SimF2.map --txt ../example/SimF2.txt --QTX 0 --out SimF2.pre
./QTXNetwork --map ../example/sorghum.map --txt ../example/sorghum.txt --QTX 0 --out sorghum.pre
./QTXNetwork --map ../example/SimF2_600.Gen --txt ../example/SimF2_600.Phe --QTX 1 --out SimF2_600.pre
./QTXNetwork --map ../example/0pca.Girth18.gen --txt ../example/0pca.Girth18.phe --QTX 1 --out 0pca.Girth18.pre

```
```
