# Dosage Calculator (Clinical Prototype)

This project is a simple, browser-based clinical calculator designed to help estimate medication dosages based on patient-specific parameters.

It is intended as a **learning project and prototype**, not as a production or prescribing tool.

---

##  Current Features

### Patient Core Metrics
The calculator currently supports calculation of:

- **Height (m)**
- **Body Mass Index (BMI)**
  - Includes BMI classification:
    - Underweight
    - Normal
    - Overweight
    - Obese
- **Body Surface Area (BSA)**
  - Formula: Mosteller

### Medication Support
- **Euthyrox (levothyroxine)**
  - Initial dose estimate based on:
    - `1.6 mcg/kg/day` (adult full replacement estimate)
  - Displayed only when Euthyrox is selected from the medication dropdown.

---

## Clinical Disclaimer

⚠️ **This tool is for educational and prototyping purposes only.**

- It does **not** replace clinical judgment.
- Medication dosing depends on many factors not yet implemented, including:
  - Age
  - Cardiac disease
  - Pregnancy status
  - Severity of disease
  - Drug interactions
  - Laboratory monitoring (e.g., TSH for levothyroxine)

Always consult official prescribing information and clinical guidelines.

---

##  How to Run

No installation required.

1. Clone or download the repository
2. Open `index.html` in any modern web browser
3. Enter:
   - Weight (kg)
   - Height (cm)
4. Select a medication (optional)
5. Click **Calculate**

---

##  Implemented Formulas

### BMI
```
BMI = weight (kg) / height (m)²
```

### BSA (Mosteller)
```
BSA = √[(height (cm) × weight (kg)) / 3600]
```

### Euthyrox Initial Dose (Prototype)
```
Dose = weight (kg) × 1.6 mcg/kg/day
```

---

##  Project Structure

```
dosage_calculator/
├── index.html    # Single-file HTML + CSS + JavaScript calculator
├── README.md     # Project documentation
└── LICENSE
```

---

## Planned Enhancements

- Severity-based levothyroxine dosing (mild vs full replacement)
- Age and cardiac risk warnings
- Tablet strength rounding suggestions
- Ideal body weight (IBW) and adjusted body weight (AdjBW)
- Additional medications with structured dosing logic
- Separation of calculation logic into reusable modules

---

##  License

This project is released under the license included in the repository.
