# Tutorial: Geospatial Data Formats

Geospatial data allows the communication of information in a wide range of fields. Over time,
many data formats have emerged to support this diversity. This tutorial introduces these various
formats, their evolution, their advantages and disadvantages, and provides guidance on how and in
which contexts to use them most effectively. It will be divided into several jupyter notebooks:

1) [Raster formats](./raster_formats.ipynb)
2) [Vector formats](./vector_data_formats.ipynb)
3) [Data cube formats](./datacube_formats.ipynb)
4) [Point clouds](./point_clouds.ipynb)
5) [Data optimization](./data_optimization.ipynb)

For each tutorial, sample data will be provided in the `sample_data` directory or automatically
downloaded (in the `sample_data` directory by default). This means that an internet connection is
required to run these notebooks. Alternatively, you can manually download data from other providers
and use them to run the notebooks. In some examples, benchmarks are ran and performances are 
compared between different formats, but the data used for these tests is generally quite small, 
mostly used as example. Using real, larger datasets highlights better the performance discrepancies
between formats. For example, in the [raster tutorial](./raster_formats.ipynb) you can use real
Sentinel-2 data, downloadable from [geodes](https://geodes-portal.cnes.fr/) or
[copernicus](https://browser.dataspace.copernicus.eu/). For the [point clouds](./point_clouds.ipynb)
 or [datacube](./datacube_formats.ipynb) tutorials, you can use SWOT data, available on
[hydroweb next](https://hydroweb.next.theia-land.fr/) (with netcdf files for example). For SWOT
data, you can also check out this tutorial (TBD).


Some notebooks showcase how to visualize the data from the different file types, but you can find 
more detailed tutorials [here](https://pluto.pages.cnes.fr/portal/data/miscellaneous/tuto_python_visu_tools_spatial_data.html).

## Installation

To run a notebook, first create a virtual environment using pip. Then, install the required 
packages (if not already done), using the `requirements.txt` file.

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Then you can simply use `jupyter notebook xxx.ipynb` to run the corresponding notebook.
