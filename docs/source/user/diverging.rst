.. _diverging:

Diverging
=========
A different category or class of colormaps, is the group of *diverging* colormaps.
Unlike sequential colormaps, diverging colormaps start at their lowest (or highest) lightness value at both ends and monotonically increase (decrease) to the highest (lowest) lightness value in the center.
This makes them very useful to represent information that has a critical middle value or when data deviates around a common center (usually zero), like topographical maps.
The *matplotlib* package has quite a few diverging colormaps, but none of them starts and ends at the same lightness value; and most do not change perceptually uniform.
Therefore, a few alternatives are introduced here.

.. _PRISM: https://github.com/1313e/PRISM


Redshift
--------
.. figure:: ../../../cmasher/colormaps/redshift/redshift.png
    :alt: Visual representation of the *redshift* colormap.
    :width: 100%
    :align: center
    :name: redshift_cmap

.. figure:: ../../../cmasher/colormaps/redshift/redshift_viscm.png
    :alt: Statistics of the *redshift* colormap.
    :width: 100%
    :align: center
    :name: redshift_viscm

The *redshift* colormap is a visual representation of the (mostly) astronomical phenomenon with the same name, where electromagnetic radiation (such as light) undergoes an increase in wavelength.
It covers almost the full lightness range (i.e., :math:`[0, 90]`) and uses red and blue as its main colors.
It is special in that, unlike most other diverging colormaps, it reaches its lowest lightness value in the center and increases in lightness towards the ends.
This makes it ideal for representing information where the deviation from the common center should be highlighted or when plotting data values where the sign of a value is used as an indicator, like in a radial velocity or rotation measure map (where the sign is an indicator of direction).
