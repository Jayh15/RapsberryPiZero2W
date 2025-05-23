# RapsberryPiZero2W
This document outlines the setup and troubleshooting steps for my Raspberry Pi Zero 2 W project. The goal was to set up the Pi with a heatsink, peripherals, and SSH access from my phone, and later enable GUI access via a display.


# Raspberry Pi Zero 2 W – Setup & SSH Access (Headless + GUI)

## Project Overview

This document outlines the setup and troubleshooting steps for my Raspberry Pi Zero 2 W project. The goal was to set up the Pi with a heatsink, peripherals, and SSH access from my phone, and later enable GUI access via a display.

---

## 📦 Hardware Used

- **Raspberry Pi Zero 2 W**
- **MicroSD Card (Flashed with Raspberry Pi OS Lite)**
- **Mini-HDMI to HDMI adapter**
- **USB OTG adapter**
- **Heatsink (applied to the main SoC)**
- **Keyboard & Mouse (initially USB accessories had issues)**
- **Display/Monitor**
- **iPhone (SSH client: Termius app)**

---

## 🛠️ Physical Setup Steps

1. **Attach Heatsink**  
   Applied to the large square chip marked with the Raspberry Pi logo (the SoC).

2. **Connect Accessories**  
   - HDMI display via mini-HDMI adapter.
   - USB keyboard and mouse via OTG adapter.
   - Note: Initial keyboard issues required multiple reboots and power re-seating.

3. **Power Up the Pi**  
   Connected via micro-USB power port (next to the HDMI port).

---

## ⚙️ Software Setup

1. **Flashed Raspberry Pi OS Lite** onto the microSD using [Raspberry Pi Imager](https://www.raspberrypi.com/software/).

2. **Enabled SSH**  
   Created an empty `ssh` file in the `/boot` partition after flashing.

   ```bash
   touch /Volumes/boot/ssh
