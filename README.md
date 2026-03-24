# Project-2-SDG-13-Climate-Action
# 🌍 SDG 13: Climate Action

## 🌱 Project: Carbon Footprint Calculator

---

## 🎯 Aim

To develop a Python-based application that estimates an individual's carbon footprint based on daily activities and provides awareness about environmental impact, supporting SDG 13 (Climate Action).

---

## 🛠️ Objectives

* To calculate carbon emissions from daily activities
* To analyze environmental impact
* To categorize carbon footprint levels
* To promote eco-friendly habits

---

## 📚 Procedure

1. Start the program
2. Prompt the user to enter monthly electricity usage (in kWh)
3. Prompt the user to enter daily travel distance (in km)
4. Prompt the user to enter number of meat-based meals per week
5. Calculate carbon emissions using approximate formulas:

   * Electricity emission = electricity × 0.85
   * Travel emission = travel × 0.21 × 30
   * Food emission = meat meals × 2.5 × 4
6. Compute total carbon footprint
7. Display total CO₂ emission
8. Classify emission level:

   * Low
   * Moderate
   * High
9. Display suggestions to reduce carbon footprint
10. Handle invalid inputs using exception handling
11. End the program

---

## 💻 Python Code

```python
print("=== Carbon Footprint Calculator ===")

try:
    electricity = float(input("Monthly electricity usage (kWh): "))
    travel = float(input("Daily travel distance (km): "))
    meat = int(input("Meat meals per week: "))

    # Emission calculations
    co2_electricity = electricity * 0.85
    co2_travel = travel * 0.21 * 30
    co2_meat = meat * 2.5 * 4

    total = co2_electricity + co2_travel + co2_meat

    print(f"\nEstimated Monthly CO2 Emission: {total:.2f} kg")

    if total < 200:
        print("🌱 Low footprint – Great job!")
    elif total < 500:
        print("⚠ Moderate footprint – Try reducing usage")
    else:
        print("🚨 High footprint – Take action to reduce emissions")

except:
    print("Invalid input! Please enter correct values.")
```

---

## ▶️ Sample Output

```
=== Carbon Footprint Calculator ===
Monthly electricity usage (kWh): 150
Daily travel distance (km): 10
Meat meals per week: 5
<img width="1496" height="795" alt="image" src="https://github.com/user-attachments/assets/a2f0de3f-e8c3-4e6a-bf37-66a6b33edd3e" />

Estimated Monthly CO2 Emission: 442.50 kg
⚠ Moderate footprint – Try reducing usage
```

---

## 🌱 SDG Mapping

This project supports:
**SDG 13 – Climate Action**

It helps users:

* Understand their environmental impact
* Track carbon emissions
* Adopt sustainable practices

---

## ✅ Conclusion

The Carbon Footprint Calculator raises awareness about environmental sustainability by estimating individual carbon emissions. It encourages users to adopt eco-friendly habits and contribute towards reducing global climate change.

---
