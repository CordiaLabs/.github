# Cordia Labs
**San Francisco, CA** · [cordialabs.io](https://cordialabs.io) · [vladimir@cordialabs.io](mailto:vladimir@cordialabs.io)

### A $1,000 robot that folds laundry.

Cloth manipulation usually fails at the point of contact. A dual-arm gripper closes, the fabric slips two millimeters, and the fold comes out crooked. Vision models miss the slip because cameras can't see pressure.

To capture this, the robot's jaws use thin-film force sensors streaming at 200 Hz. The contact data is hardware-synced with the camera views and joint states, and written straight to LeRobot's dataset format. When a fold fails, the slip is in the log.

Target is $1,000. Collecting usable cloth data requires putting robots in actual laundry rooms instead of a single lab, so the rig has to be cheap enough to distribute.

V0 is built and teleoperating. I'm based in the Bay Area and looking for local commercial laundry operations to host an early pilot.

---

## Public Repositories

| Repository | Description | License |
|---|---|---|
| [**`tactile-firmware`**](https://github.com/CordiaLabs/tactile-firmware) | ESP32 firmware streaming thin-film FSR contact pressure at 200 Hz (<$10/hand) | Apache-2.0 |
| [**`teleop-stack`**](https://github.com/CordiaLabs/teleop-stack) | Dual SO-101 teleoperation, cameras, and tactile data logging in LeRobot dataset format | Apache-2.0 |
| [**`v0-cad`**](https://github.com/CordiaLabs/v0-cad) | CAD models, STEP source, and 3D printable parts for the mobile cart bench | CERN-OHL-S-2.0 |

---

## V0 Build Specifications

| Subsystem | Specification |
|---|---|
| **Kinematics** | Dual SO-101, Feetech STS3215 over serial bus |
| **Vision** | Overhead 720p, cropped to roughly 78 cm at about 1.3 mm per pixel, plus two wrist views, referenced to the arm base rather than the room |
| **Tactile** | ESP32 plus thin-film FSRs at 200 Hz, under $10 per hand |
| **Logging** | Vision, joint state, and contact synced to one clock, written to LeRobot format |
| **First Garments** | T-shirts, hand towels, pillowcases |

---

## Pilots & Inquiries

If you run a drop-off laundry, a hotel laundry, or a turnover crew and want to try one, email: [vladimir@cordialabs.io](mailto:vladimir@cordialabs.io)
