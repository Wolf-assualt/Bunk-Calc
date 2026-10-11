# 🎓 Bunk Calculator

A lightweight, client-side web application designed to help students track attendance and calculate how many classes they can safely skip or need to attend to satisfy their required attendance criteria.

---

## 📌 Features

* **Live Attendance Calculation**: Computes your current percentage instantly based on total and attended classes.


* **Bunk Estimator**: Calculates how many upcoming lectures you can safely miss while remaining at or above your target threshold.


* **Catch-Up Calculator**: Determines the exact number of consecutive classes you must attend to recover from a low attendance percentage.


* **Visual Status Feedback**: Color-coded indicators and a dynamic progress bar for **Safe**, **Borderline**, and **Danger** states.


* **Zero Dependencies**: Built with pure HTML, CSS, and Vanilla JavaScript—runs locally in any browser without external packages or server setups.



---

## 🧮 Mathematical Formulas

The application calculates attendance dynamics using the following formulas:

### 1. Classes You Can Safely Bunk

When your current attendance meets or exceeds the required threshold ($A / T \ge r$):

$$\text{Bunks Allowed} = \left\lfloor \frac{A}{r} - T \right\rfloor$$

### 2. Consecutive Classes Needed to Catch Up

When your current attendance falls below the required threshold ($A / T < r$):

$$x = \left\lceil \frac{r \cdot T - A}{1 - r} \right\rceil$$

Where:

* $A$ = Classes attended so far


* $T$ = Total classes held so far


* $r$ = Target attendance percentage in decimal form (e.g., $0.85$ for $85\%$)


* $x$ = Minimum consecutive classes required to reach $r$

---

## 🚀 Getting Started

### Prerequisites

* Any standard web browser (Chrome, Firefox, Safari, Edge, or Brave).

### Installation & Usage

1. Clone the repository:
```bash
git clone https://github.com/your-username/bunk-calculator.git

```


2. Open the project folder:
```bash
cd bunk-calculator

```


3. Open `bunk-calculator.html` in your web browser:
```bash
# Linux
xdg-open bunk-calculator.html

# macOS
open bunk-calculator.html

# Windows
start bunk-calculator.html

```



---

## 🛠️ Tech Stack

* **HTML5**: Semantic forms and document structure.


* **CSS3**: Centered card layout, rounded input elements, and status alerts.


* **JavaScript (ES6+)**: Input validation, real-time math evaluation, and DOM updates.



---

## 📄 License

This project is open-source and licensed under the [MIT License](https://www.google.com/search?q=LICENSE).
