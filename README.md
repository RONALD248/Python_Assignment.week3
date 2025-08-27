# Discount Calculator Program

##  Description

This program calculates the final price of an item after applying a discount.

* If the discount percentage is **20% or higher**, the discount is applied.
* If the discount percentage is **less than 20%**, no discount is applied and the original price is returned.

It demonstrates the use of:

* **Functions**
* **Conditional statements (`if`/`else`)**
* **User input and output**

---

##  How It Works

1. The user is prompted to enter:

   * The original price of the item.
   * The discount percentage.
2. The program checks if the discount is 20% or more:

   * ✅ If yes → It applies the discount and prints the final price.
   * ❌ If not → It prints the original price without changes.

---

## 🖥 Example Usage

```
Enter the original price of the item: 1000
Enter the discount percentage: 25
The final price after 25.0% discount is: 750.0
```

```
Enter the original price of the item: 800
Enter the discount percentage: 15
No discount applied. The price remains: 800.0
```

---

##  Code

```python
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        final_price = price - (price * discount_percent / 100)
        return final_price
    else:
        return price


price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

final_price = calculate_discount(price, discount_percent)

if discount_percent >= 20:
    print(f"The final price after {discount_percent}% discount is: {final_price}")
else:
    print(f"No discount applied. The price remains: {final_price}")
```

---

##  How to Run

1. Save the code into a file called **discount\_calculator.py**.
2. Open a terminal or command prompt.
3. Run the program using:

   ```
   python discount_calculator.py
   ```
4. Follow the prompts to enter the price and discount.

---


