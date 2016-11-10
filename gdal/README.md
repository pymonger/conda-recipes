# gdal-2.1.0 built with expat support (enable reading of KML)

## Build
conda build gdal
conda install --use-local gdal
conda convert --platform all ~/anaconda3/conda-bld/linux-64/gdal-2.1.0-py35_0.tar.bz2 -o outputdir/

## Upload
anaconda login
anaconda upload ~/anaconda3/conda-bld/linux-64/gdal-2.1.0-py35_0.tar.bz2
