This project is a mini assignment on **Association Rule Mining** using the **Apriori algorithm**. It involves simulating shopping transaction data, analyzing frequent itemsets, and generating association rules to discover common shopping patterns.

---

##  Assignment Overview

**Objective:**  
To simulate basic transactional data and use association rules to uncover relationships between items commonly bought together.

**Tasks Completed:**
1. Simulated 10 fake transactions using 8 unique items.
2. Converted the data into one-hot encoded format using pandas.
3. Used the Apriori algorithm to find frequent itemsets with at least 30% support.
4. Generated association rules with at least 70% confidence.
5. Selected one rule and explained its meaning in real life.

---

## Simulated Items and Transactions

**Item Pool:**
- Bread, Milk, Eggs, Cheese, Apples, Diapers, Beer, Coke

**Number of Transactions:**
- 10 (each transaction contains 2 to 5 randomly selected items)

---

##  Frequent Itemsets (Support ≥ 0.3)

Here are some itemsets that were found to be frequent (appear in at least 30% of transactions):

| Itemset           | Support |
|-------------------|---------|
| Eggs              | 0.7     |
| Beer              | 0.5     |
| Diapers           | 0.5     |
| Bread             | 0.4     |
| Cheese            | 0.3     |
| Apples            | 0.3     |
| Eggs & Beer       | 0.4     |
| Bread & Eggs      | 0.3     |
| Diapers & Cheese  | 0.3     |

This means, for example, **Eggs** appeared in 70% of all the transactions, making it the most common item.

---

##  Association Rules (Confidence ≥ 0.7)

Here are the top rules generated from the frequent itemsets:

| Rule                     | Confidence | Lift |
|--------------------------|------------|------|
| If Beer → then Eggs      | 0.80       | 1.14 |
| If Bread → then Eggs     | 0.75       | 1.07 |
| If Cheese → then Diapers | 1.00       | 2.00 |

---

##  Chosen Rule Explanation

**Rule:**  
If someone buys `Beer`, they are likely to also buy `Eggs`.

**Confidence:**  
0.80 (This means the rule holds true 80% of the time.)

**Real-Life Meaning:**  
This rule shows that people who buy **Beer** also tend to buy **Eggs**. In a supermarket, this insight can help decide how to place items on shelves or what to bundle in promotions. For example, putting Beer and Eggs closer together might increase sales.

---

##  How to Run the Code

### Requirements
- Python 3
- pandas
- mlxtend

### Steps

1. Install dependencies:

```bash
pip install pandas mlxtend
