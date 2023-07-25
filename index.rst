:tocdepth: 1

.. sectnum::

.. Metadata such as the title, authors, and description are set in metadata.yaml

Abstract
========

This technote focuses on analyzing the system static flexure as a function of elevation, derived from the Laser Tracker measured offsets. It will be updated once data is available to include LUT improvement for the hexapods. For now, this is not possible because the Laser Tracker data was obtained without the hexapods being turned on nor the M2 surrogate being in place.


Current Hexapod LUT
=====================

Let us first start by looking at the Hexapod LUT that we currently have in place. Below are the LUT offsets as a function of the elevation angle for the camera and the M2 Hexapod.

.. figure:: /_static/camera_lut.png
   :name: camera_lut

.. figure:: /_static/m2_lut.png
   :name: m2_lut


Laser Tracker Offsets
=======================

The first Laser Tracker sequence was run on July 5th, 2023. It was a step-wise slew that went from 0 to 90 deg and back to 0 deg, to ensure hysteresis was covered in the offsets. The telescope was stopped at every 5 deg, and the Laser Tracker align sequence was then run for both the camera and the M2. See below the elevation plot while running this sequence.

.. figure:: /_static/elevations.png
   :name: elevations
   :scale: 50 %

That sequence generated a set of offsets that were used to realign the system. Looking at those offsets we can drive conclusions on the system flexure. Below are the Camera Offsets measured by the Laser Tracker.

.. figure:: /_static/camera_offsets.png
   :name: camera_offsets

Below are the M2 Offsets measured by the Laser Tracker.

.. figure:: /_static/m2_offsets.png
   :name: m2_offsets

Interestingly, we see that the measured offsets are very similar to the current LUT, but they show certain differences that are probably due to the LUT inaccuracy and the fact that these offsets were measured with a system that did not have all the components it will consist of.

Next steps
=======================

Since the M2 surrogate was not in place, and neither the two hexapods were turned on, the conclusions that we can derive are limited. When all the pieces are in place, we will be able to repeat this procedure and update the system LUT by looking at the Laser Tracker offsets.
