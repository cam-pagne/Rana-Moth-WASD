# The Rana Labs Moth (WASD Version)

My version of Rana Labs' Moth controller, a foldable leverless controller.

---

## Shell Prints

I printed the entire shell, hinges, etc., in **Bambu Lab PETG**, though any PETG should work. I printed the hinge pin with **PLA+**, as PETG would warp without supports.

- **Microcontroller:** Standard Pico, screws in with any **M2 screws** (4mm length, but shorter would work).
- **Switches:** Must be **low profile switches**. I used **Cosmox Wind Engines** and a couple **KS33 Silvers**.
- **USB-C Connector:** Model UD (superglued in), but I recommend using **ModelBirdD** for mounting with screws. You'll need to modify the model slightly to fit ModelBirdD.

---

## Assembly Instructions

1. **Pre-Wiring:**
   - Wire up the **Pico side completely** first.
   - Then, individually run the wires from the opposite side one by one.
   - **Important:** Do this while the Moth is in the **folded position!**

2. **Wiring Tips:**
   - If not folded while soldering cross-body wires, they might be pulled too tightly when folding.
   - Leave **decent slack** for cross-body wiring.
   - Pass wires behind the hinge pin for neatness.

3. **Hinge Pin Placement:**
   - Insert the hinge pin **before** wiring the cross-body connections.
   - Attempting to run wires before inserting the hinge pin can make installation difficult, the wires will block the pin from going through.

---

## Magnets

Strong magnets are crucial, as they counteract the springs in your switches. I used:

- **6x2mm Neodymium magnets**, stacked **3 high** in each of the **10 total holes** (30 total magnets).
- These create a satisfying snap and keep the Moth securely folded.

**Amazon link:** [Magnets used](https://a.co/d/aDkEUHX)

---

## Folded Design

For the reverse folded position:

- A **lip** on the top hinge piece prevents overfolding, creating a stopping point.
- Hinges have a rounded back that creates friction, providing rigidity while playing in the ergonomic 'prism' setup.

### Adjustments:

- You can edit the lip's width to adjust the folding angle.
- Recommended change: **Move the lip from the top to the bottom hinge**, because:
  - The top hinge cannot be removed without complete rewiring.
  - The bottom hinge allows for hinge pin removal, making angle changes easier.

---

## Miscellaneous Notes

- **Button Fit:** Ensure buttons sit flush with the face surface when depressed to allow proper folding.
- **Magnet Strength:** Strong neodymium magnets may overcome minor protrusions but aim for flush alignment.
- **Hinge Pin Slot:** You can add caps for a cleaner look, but friction fit holds securely without them.

---

## Adding Images to GitHub

To add images to your GitHub project, follow these steps:

1. Create an `images/` folder in your project repository.
2. Upload your images to the folder.
3. Use Markdown syntax to embed images in your README:
   ```markdown
   ![Description of Image](images/filename.jpg)
