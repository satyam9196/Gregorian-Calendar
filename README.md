# Gregorian-Calendar

# 📅 Gregorian to Hypothetical 13-Month Calendar Converter (1582–3000)

This project provides a dataset and conversion logic for mapping **Gregorian calendar dates** (from the year **1582 to 3000**) to a **hypothetical 13-month calendar** system. It is designed for experimentation in timekeeping systems, simulations, data science tasks, and educational demonstrations.

---

## 📌 What is a 13-Month Calendar?

The 13-month calendar divides the year into:
- **13 months of 28 days each** (364 days)
- **1 "Year Day"** (or 2 in a leap year) not assigned to any month or week

This system creates perfect **4-week months**, with each month starting on the same weekday every year.

---

## 📊 Dataset Overview

| Column | Description |
|--------|-------------|
| `Gregorian_Date` | Date in standard Gregorian format (YYYY-MM-DD) |
| `13Month_Year` | Corresponding year in the 13-month system |
| `13Month_Month` | Month (1 to 13) |
| `13Month_Day` | Day of the month (1 to 28) |
| `Day_Type` | `Normal`, `Year Day`, or `Leap Day` |
| `Weekday` | Day of the week (e.g., Monday) |
| `Is_Leap_Year` | Boolean indicating whether it's a leap year |

✅ **Date range:** 1582-10-15 to 3000-12-31  
📄 **File format:** CSV  
📁 **Dataset size:** ~520,000+ records

---

## 📂 Files Included

- `Gregorian_to_13Month_Calendar.csv`: Full dataset (Gregorian to 13-month mapping)
- `calendar_converter.ipynb`: Jupyter notebook with conversion code, visualizations, and calendar logic
- `README.md`: Project documentation

---

## 🧮 Core Logic

- Leap years handled per **Gregorian calendar rules** (every 4 years, except centuries not divisible by 400)
- Conversion maintains alignment with weekdays
- "Year Day" inserted after the 364th day
- Optional leap day inserted after June or December, depending on chosen design

---

## 📈 Example

| Gregorian Date | 13Month Date | Day Type   |
|----------------|---------------|------------|
| 2025-01-01     | 2025-M01-D01  | Normal     |
| 2025-12-28     | 2025-M13-D28  | Normal     |
| 2025-12-29     | -             | Year Day   |

---

## 🚀 Use Cases

- Chronological data normalization  
- Alternate calendar studies  
- Data science or AI models needing consistent month structures  
- Time simulation or game design  
- Educational tools for teaching calendar reform concepts

---

## 🧑‍💻 Author

**Satyam9196**  
🔗 GitHub: [@satyam9196](https://github.com/satyam9196)

---

## 📜 License

This project is open-source under the [MIT License](LICENSE).

---

## 🙌 Contributions

Found a bug or want to add enhancements? Pull requests are welcome!

