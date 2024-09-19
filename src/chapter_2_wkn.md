# Well Known Nodes

![Map, as of September 18th, 2024](./images/tehachapi-meshtastic-map-20240918.png)

## Downtown Tehachapi

### `dt01` / `downtown-01`

Operates from downtown, historically stable and backed by a UPS unit. The
antenna placement is sub-optimal, but seems to generally get about a mile
of coverage.

- **Hardware:** [2019 LILYGO T-Beam T22 v1.1](https://meshtastic.org/docs/hardware/devices/tbeam/?t-beam=1.1)
- **Software:**  [Meshtastic Firmware v2.4.2.5b45303](https://github.com/meshtastic/firmware/releases/tag/v2.4.2.5b45303)
- **Mode:** `CLIENT`

Software gets updated along the Beta channel semi-frequently, and this documentation does not automatically update.

## Alpine Forest

### `av01` / `alpine-village-01`

Operates from the South East side of Alpine Forest (sometimes called Alpine
Village), near Indian Hills Campground, that's generally stable and backed
by a UPS unit. The antenna placement is sub-optimal. This is in a small valley
base, so coverage is limited.

- **Hardware:** [2019 LILYGO T-Beam T22 v1.1](https://meshtastic.org/docs/hardware/devices/tbeam/?t-beam=1.1)
- **Software:**  [Meshtastic Firmware v2.4.2.5b45303](https://github.com/meshtastic/firmware/releases/tag/v2.4.2.5b45303)
- **Mode:** `CLIENT`

Software gets updated along the Beta channel semi-frequently, and this documentation does not automatically update.

### `rs04` / `rak-solar-04` 

Operates from the South East side of Alpine Forest (sometimes called Alpine
Village), near Indian Hills Campground.

- **Hardware:** [2024 RAK4631](https://meshtastic.org/docs/hardware/devices/rak/)
  - **Power:** Solar + 5Ah Battery
    - **Antenna:** External Fiberglass
- **Software:**  Close to [Meshtastic Firmware v2.4.2.5b45303](https://github.com/meshtastic/firmware/releases/tag/v2.4.2.5b45303).
- **Mode:** `CLIENT` (Potentially may become `ROUTER` for the area, if nothing better is found)

Software gets updated along the Beta channel semi-frequently, and this documentation does not automatically update.

### `rs01` / `rak-solar-01` 

Operates from the South East side of Alpine Forest a few hundred feet above
`rs04` with a strong view of the Western side of Tehachapi Mountain.
Undergoing testing for permanent installation, but I'll need to see how it
does over the winter.

- **Hardware:** [2024 RAK4631](https://meshtastic.org/docs/hardware/devices/rak/)
  - **Power:** Solar + 3Ah Battery
  - **Antenna:** Internal
- **Software:**  Close to [Meshtastic Firmware v2.4.2.5b45303](https://github.com/meshtastic/firmware/releases/tag/v2.4.2.5b45303).
- **Mode:** `CLIENT`

## Jury Ranch

### `jr01` / `jury-ranch-01`

Operates from a location on Jury Ranch, and generally acts as a bridge across
the ridgelines separating Line-of-Sight between the East and Western halves
of Tehachapi Valley.

- **Hardware:** [2024 RAK4631](https://meshtastic.org/docs/hardware/devices/rak/)
  - **Power:** Solar + 3Ah Battery 
  - **Antenna:** Internal
- **Software:**  Close to [Meshtastic Firmware v2.4.2.5b45303](https://github.com/meshtastic/firmware/releases/tag/v2.4.2.5b45303).
- **Mode:** `CLIENT` (Slated to change to `ROUTER` or `REPEATER`)
- **Formerly Known As:** `rs03` / `rak-solar-03`