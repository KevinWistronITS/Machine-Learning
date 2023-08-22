# Feature Scaling

### Prerequisite
N/A

### Feature Scaling Type

1. Normalization
    
    ![Normalization](/pic/Normalization.png)
    
> Your value should be between 0 and 1. `[0;1]`
    
1. Standardization
    
    ![Standardization](/pic/Standardization.png)
    
> Your value should be between 3 and -3. `[-3;3]`
    
For example,

|  | Salary (USD) | Age (yrs) |
| --- | --- | --- |
| A | $70000 | 45 |
| B | $60000 | 44 |
| C | $52000 | 40 |

After normalization:

|  | Salary (USD) | Age (yrs) |
| --- | --- | --- |
| A | 1 | 1 |
| B | 0.44 | 0.8 |
| C | 0 | 0 |

---
Next &rarr; [Data Preprocessing](/Day-1/Day1-Data-Preprocessing.md)
Previous &larr; [Machine Learning](/Day-1/Machine-Learning.md)