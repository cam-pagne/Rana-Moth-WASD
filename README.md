# The Rana Labs Moth (WASD Version)

WASD version of [Rana Labs'](https://github.com/rana-sylvatica) Moth, a foldable leverless controller.

<div style="display: flex;">
    <img src="Images/PCB Moth - White.jpg" alt="Layout 1" width="600" />
</div>

<details>
  <summary><h4>What's changed from the original?</h4></summary>

- Added the WASD style up button.
- Sunk part of the shell under the WASD cluster to add mounting points for the Raspberry Pico.
- Removed one modifier button and repositioned the others for increased comfort.
- Changed the USB-C port location to accommodate the WASD layout (port slot fitted for ModelUD).
- Enlarged the hinge rounded edges to ensure a secure friction fit in 'prism' mode.
- Added a lip to the hinge to lock in the desired prism angle.
- Adjusted the thickness of the hinge pin holes for a tighter friction fit.
- Modified the magnet hole size to accommodate larger magnets that firmly snap the controller together.
- Filleted the controller edges to provide a smoother, rounded feel.

</details>

---

## Build Overview

I printed the entire shell, hinges, etc., in **Bambu Lab PETG** (though any PETG or PLA should work). The hinge pin was printed with **PLA+** since PETG tends to warp without supports.

- **Microcontroller:** RP2040—**integrated directly onto the custom PCB.** No separate soldering is needed for the Pico if using my PCB design.
- **Switches:** Must be **low profile switches.** I use pretty much any Kailh Choc Low Profile switches. They all work, just choose a preferred switch type.
- **USB-C Connector:** [Model UD](https://github.com/HTangl/Model-UD) (superglued in). For a screw-mounted option, consider the **Model BirdD** (requires slight model modifications).

---

## Assembly Options

### PCB Option

To streamline your build, I’ve designed a custom PCB for this controller. This board integrates the Pico directly—eliminating the need for any handwiring of the microcontroller. The **only soldering required is the installation of the hotswap sockets for the Choc switches.** This approach not only simplifies assembly but also reduces the potential for wiring errors.

The two halves of the board are connected using a 20 pin, .5 pitch ribbon cable, and the QuRB is connected to the Left side board for USB C port via a 12 pin, .5 pitch ribbon cable.

<details>
  <summary><strong>Handwiring Option (Optional)</strong></summary>

For users who prefer a traditional approach or as a reference, here are the handwiring instructions. (Note: When using the PCB option, this process is unnecessary.)

### Initial Wiring:
- **Pico Side:** Wire up the Pico side completely first.
- **Opposite Side:** Run the wires individually from the opposite side.
- **Important:** Ensure that you run the cross-body wiring while the Moth is in its **folded position** to avoid tension.

### Wiring Tips:
- If the controller isn’t folded during soldering, the cross-body wires may become too tight when folding later.
- Leave **ample slack** for the cross-body wiring.
- Route wires behind the hinge pin for a neat installation.

### Hinge Pin Placement:
- Insert the hinge pin **before** wiring the cross-body connections.
- Running wires prior to inserting the hinge pin can obstruct its path, making installation challenging.

#### Wiring Example

This was my first soldering project in a long time; while my solder joints may not be perfect, the key point is the proper routing of wires from the non-Pico side to the Pico side.
<div style="display: flex;">
    <img src="Images/Wiring Example.jpg" alt="Wiring Example" width="500" />
</div>

</details>

---

## Magnets

Strong magnets are crucial, as they must counteract every spring in your switches. I used:

- **6x3mm Neodymium magnets**, stacked **2 high** in each of the **10 total holes** (20 magnets overall).
- This setup creates a satisfying snap and keeps the Moth securely folded.

**Amazon link:** [Magnets used](https://www.amazon.com/dp/B096LZNZTQ?ref=cm_sw_r_cp_ud_dp_ZEAK3BD945P57Y9BB6P4&ref_=cm_sw_r_cp_ud_dp_ZEAK3BD945P57Y9BB6P4&social_share=cm_sw_r_cp_ud_dp_ZEAK3BD945P57Y9BB6P4&skipTwisterOG=1&newOGT=1&th=1)

---

## 'Prism' Ergonomic Mode

For the reverse folded position:

- A **lip** on the two hinge pieces prevents overfolding by creating a defined stopping point.
- The rounded back of the hinges generates friction, ensuring rigidity in the ergonomic 'prism' configuration.

### Adjustments:

- The hinge lip’s width can be edited to modify the folding angle.

---

## Miscellaneous Notes

- **Button Fit:** Ensure buttons sit flush with the face surface when pressed to allow proper folding.
- **Magnet Strength:** Although strong neodymium magnets can overcome minor misalignments, aim for a flush fit.
- **Hinge Pin Slot:** While you can add caps for a cleaner look, the friction fit alone holds securely.

---
