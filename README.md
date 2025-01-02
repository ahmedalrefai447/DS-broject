# DS-broject
## Team 
- ahmed alrefai
- yacoub abubaker
- python
# Import the required libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Step 1: Create a DataFrame with 50 rows and 2 columns
np.random.seed(0)
data = {
    'Column1': np.random.randint(1, 100, 50),
    'Column2': np.random.randint(1, 100, 50)
}
df = pd.DataFrame(data)

# Step 2: Perform some calculations
average_column1 = df['Column1'].mean()
average_column2 = df['Column2'].mean()

# Step 3: Visualize the data
plt.figure(figsize=(10, 5))
plt.plot(df['Column1'], label='Column1', color='blue')
plt.plot(df['Column2'], label='Column2', color='orange')
plt.xlabel('Index')
plt.ylabel('Values')
plt.title('Line Plot of Column1 and Column2')
plt.legend()
plt.savefig('output.png')
plt.show()

# Save the DataFrame to a CSV file
df.to_csv('data.csv', index=False)

# Print calculated values
print(f"Average of Column1: {average_column1}")
print(f"Average of Column2: {average_column2}")

## Dataset Details
The dataset contains 50 rows and 2 columns:
- **Column1**: Random integers between 1 and 100.
- **Column2**: Random integers between 1 and 100.

## Functions and Classes

### Functions
- **main()**
  - **Description**: The main function that calls other functions.
  - **Methods**: 
    - **Data Creation**: Generates a dataset with 50 rows and 2 columns.
    - **Data Visualization**: Uses Matplotlib to visualize the data.

### Loops
- **for loop**: Used to iterate over the DataFrame rows.
- **while loop**: Not used in this project.

### Conditional Statements
- **if statement**: Used to check certain conditions before performing calculations.

## Code Inputs and Outputs

### Inputs
- The code generates a dataset of random integers.

### Outputs
- **data.csv**: The generated dataset.
- **output.png**: The line plot of the dataset.
- **Printed Output**: Average values of Column1 and Column2.
