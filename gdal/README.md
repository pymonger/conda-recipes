# gdal-2.1.0 built with expat support
The default gdal conda package is not able to read KML:

https://github.com/conda/conda/issues/2398

This conda package solves that issue by building gdal-2.1.0 with expat support.


## Installation
```
conda install -c gmanipon gdal
```


## Build
```
conda build gdal
conda install --use-local gdal
conda convert --platform all ~/anaconda3/conda-bld/linux-64/gdal-2.1.0-py35_0.tar.bz2 -o outputdir/
```


## Upload
```
anaconda login
anaconda upload ~/anaconda3/conda-bld/linux-64/gdal-2.1.0-py35_0.tar.bz2
```
