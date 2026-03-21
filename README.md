# atlas_fume_extraction
An extraction blower fan for removing harmful fumes while soldering.


# High-Speed Centrifugal Fume Extractor
An engineering project focused on high-velocity air filtration using a custom 25,000 RPM motor and a CAD designed, 3D-printed volute housing.

## 🛠 System Architecture
![System Architecture](box_diagram_EF.drawio.png)

## 📋 Technical Specifications
* **Motor:** 25,000 RPM High-Speed DC Motor
* **Power:** 12V/24V DC Input
* **Safety:** 12A 250V Cartridge Fuse (In-line)
* **Protection:** Flyback Diode (D702) & Bulk Capacitance (C201)
* **Housing:** Custom PLA Volute (Designed in Onshape)
* **Filtration:** 100mm Activated Carbon Sheet

## ⚡ Electronics Notes (Scavenged Components)
The power conditioning circuit utilizes components salvaged from a Chicony switch-mode power supply:
1. **Flyback Diode (D702):** Protects the PWM controller from high-voltage inductive spikes (Back-EMF) during motor deceleration.
2. **Bulk Capacitor (C201):** Smooths voltage ripple and provides current "headroom" for the 12A startup surges.

## 🏗 Build Instructions
1. **CAD:** Export the volute and impeller from Onshape as .STL files.
2. **Print:** Use PLA with 3+ walls for structural rigidity against motor vibration.
3. **Wiring:** Follow the `box_diagram_EF.drawio` map. **Note:** Ensure the D702 diode stripe (Cathode) is connected to the Positive rail.
