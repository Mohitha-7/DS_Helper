DS_Helper Project
Week 1 – Column Type Detector  

- Implemented in **`column_detector.py`**.  
- Function: `detect_column_types(df)`  
- Logic:  
  - **Numerical columns** → detected using pandas numeric types.  
  - **Categorical columns** → identified if the number of unique values < threshold.  
  - **Text columns** → detected if dtype is `object` or `string`.  

Example Output (Titanic Dataset)  
```python
{
  'PassengerId': 'numerical',
  'Survived': 'categorical',
  'Pclass': 'categorical',
  'Name': 'text',
  'Sex': 'text',
  'Age': 'numerical',
  'SibSp': 'categorical',
  'Parch': 'categorical',
  'Ticket': 'text',
  'Fare': 'numerical',
  'Cabin': 'text',
  'Embarked': 'text'
}
