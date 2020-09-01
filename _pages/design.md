---
permalink: /design/
title: "KAPA Design"
---

KAPA upgrades the LMCT LGS single-conjugate adaptive optics (SCAO) system to
a 4-laser tomographic AO system (LTAO). KAPA offers three fundamental
improvements over the existing AO system:

* **Higher Strehl** is achieved through the use of four LGS for
atmospheric tomography to eliminate the “cone effect”.
* **More Sky Coverage** is achieved by using partially AO-corrected near-infrared tip-tilt stars for low-order correction.
* **Accurate PSFs** are achieved by deploying new reconstruction techniques that use AO telemetry, atmospheric profiling, and extensive instrument calibrations.


## Science Instrument
KAPA’s gains will be delivered to the existing OSIRIS science
instrument, which provides diffraction-limited, near-infrared imaging
and integral field spectroscopy (IFS) that is needed by all four
science cases.

## Hardware Changes
The changes required for atmospheric tomography include:
1. Replacing the existing laser on the Keck I Nasmyth platform with a
   TOPTICA/MPBC fiber laser on the elevation ring for sufficient sodium return.
2. Implementing a rotating 4 LGS asterism as part of the beam train.
3. Implementing a new wavefront sensor camera, specifically a lower
noise, larger format OCAM2k camera with four sets of pupil relay
optics.
4. Implementing a new real-time controller to support laser
tomography.
5. Upgrading the existing controls and operations software.
6. Algorithm changes to the near-infrared TT sensor.
7. Developing an operational PSF-R compute facility.

## Laser Guide Stars
KAPA includes the implementation of a TOPTICA Raman-fiber amplifier
laser on the Keck I telescope to replace the existing Lockheed Martin
Coherent Technology laser. The existing Keck I laser, with an
equivalent sodium return of R = 9.2 to 9.7 magnitude, is not bright
enough to be divided into multiple beacons. The existing Keck II
TOPTICA laser typically has the equivalent return of a R = 7.4
star. Splitting its 22 W of laser power into three 7 W beacons would
result in R = 8.7 stars (the return has been measured to be linear
with power). The predicted performance versus LGS asterism radius is
shown below. A 6.35 arcsec radius has been selected for KAPA,
as limited by the detector.

<figure class="half">
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/lgs_radius.png">
        <img src="{{ site.url }}{{ site.baseurl }}/assets/images/lgs_radius.png">
    </a>
    <figcaption>KAPA Improvement in Wavefront Error vs. LGS Asterism Radius</figcaption>
</figure>

<!-- This section still references the old 3 LGS plan -->


