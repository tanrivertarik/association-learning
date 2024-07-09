## Apriori Association Rule Learning from Scratch (Python)

This project implements the Apriori algorithm for association rule learning without relying on external libraries like scikit-learn. It helps discover frequent itemsets and generate association rules to understand relationships between items in transaction data.

**Features:**

- Implements the Apriori algorithm for frequent itemset generation and association rule creation.
- Allows you to specify minimum support and confidence thresholds to filter results.

**Requirements:**

- Python (version 3.x recommended)

**Usage:**

1. Clone this repository to your local machine.
2. Open a Python terminal or IDE and navigate to the project directory.
3. Modify the script (`apriori.py`) to provide your transaction data as a list of itemsets or a path to your data file (CSV format recommended).
4. Run the script with optional arguments for minimum support and confidence thresholds:

   ```bash
   python apriori.py [data_path] [min_support] [min_confidence]
   ```

   - `data_path` (optional): Path to your CSV file containing transaction data (each row representing an itemset). If not provided, sample data will be used.
   - `min_support` (optional): Minimum support threshold (default: 0.1).
   - `min_confidence` (optional): Minimum confidence threshold (default: 0.5).

**Output:**

The script will print the discovered frequent itemsets and the generated association rules based on the specified thresholds.

**Example:**

To perform association rule learning on a CSV file named "transactions.csv" with a minimum support of 0.2 and minimum confidence of 0.7:

```bash
python apriori.py transactions.csv 0.2 0.7
```

**Implementation Details:**

- The code will likely define functions for:
    - Reading transaction data from a file or using a provided list.
    - Calculating support for each itemset.
    - Generating candidate itemsets based on frequent itemsets.
    - Pruning non-frequent candidates using the Apriori property.
    - Generating association rules from frequent itemsets and calculating their confidence.

**Additional Notes:**

- This implementation offers a deeper understanding of the Apriori algorithm's mechanics.
- It may be less efficient for large datasets compared to optimized libraries like scikit-learn.
- You can extend the code to handle larger datasets, filter results by itemset length, or visualize the discovered relationships.

**Contributing:**

Feel free to submit pull requests with enhancements, optimizations, or bug fixes!

**License:**

This project is licensed under the MIT License (see LICENSE file for details).

