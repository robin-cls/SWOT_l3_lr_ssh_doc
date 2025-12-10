V1.0.0 changes
==============

This note is not exhaustive and does not reflect all the changes brought to the
product from V0.3 to V1.0.0

Basic and Expert
++++++++++++++++

.. _osm-mask:

Land-sea mask
-------------

The mask provided in the L2 product is sometimes incorrect (known limitation,
regionally dependent). A tentative improvement was done in v1.0 with the use of
a mask derived from Open Street Map (OSM).

.. image:: changes_1.0.0_masks.png
  :align: center
  :width: 800

.. note::

    The mask only changed in the 2km dataset. The 250m dataset still uses the
    land/sea mask from the Level-2 product
    ``ancillary_surface_classification_flag``
