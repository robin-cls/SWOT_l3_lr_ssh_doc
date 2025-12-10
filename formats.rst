Data formats
************

This section presents the data storage formats used for the products. The
official diffusion format is Netcdf.

Netcdf
++++++

The official products are stored using the NetCDF format.

NetCDF (network Common Data Form) is an interface for array-oriented data access
and a library that provides an implementation of the interface. The netCDF
library also defines a machine-independent format for representing scientific
data. Together, the interface, library, and format support the creation, access,
and sharing of scientific data. The netCDF software was developed at the Unidata
Program Center in Boulder, Colorado. Please see
`Unidata NetCDF <https://www.unidata.ucar.edu/software/netcdf/>`_ pages for more
information and to retrieve the NetCDF software package.

NetCDF data is:
  * Self-Describing. A netCDF file includes information about the data it
    contains
  * Architecture-independent. A netCDF file is represented in a form that can be
    accessed by computers with different ways of storing integers, characters, and
    floating-point numbers
  * Direct access. A small subset of a large dataset may be accessed efficiently,
    without first reading through all the preceding data
  * Appendable. Data can be appended to a netCDF dataset along one dimension
    without copying the dataset or redefining its structure. The structure of a
    netCDF dataset can be changed, though this sometimes causes the dataset to be
    copied
  * Sharable. One writer and multiple readers may simultaneously access the same
    netCDF file.

The products are stored in NetCDF defined by the Cooperative Ocean/Atmosphere
Research Data Service (COARDS) and Climate and Forecast (CF) metadata
conventions. The CF convention generalises and extends the COARDS convention but
relaxes the COARDS constraints on dimension and order and specifies methods for
reducing the size of datasets. A wide range of software is available to write or
read NetCDF/CF files.

API are made available by `UNIDATA <http://www.unidata.ucar.edu/software/netcdf>`_:
  * C/C++/Fortran
  * Java
  * MATLAB, Objective-C, Perl, Python, R, Ruby, Tcl/Tk


File nomenclature
-----------------

The nomenclature used for the products is:

SWOT_L3_LR_SSH_<FileIdentifier>_<CCC>_<PPP>_<DateBegin>_<DateEnd>_v<Version>.nc

where
  * FileIdentifier is ``Basic`` or ``Expert`` or ``Unsmoothed``
  * CCC is the number of cycle on 3 digits
  * PPP is the number of pass on 3 digits
  * DateBegin and DateEnd are the begin and end dates in UTC of the measurements
    in each file.
  * Version is the numerical version ``x.y.z`` with three digits refering to one
    of the :ref:`releases<releases>` (ex. ``3.0.0``)
