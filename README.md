# 🧼 Task 1: Data Cleaning and Preprocessing

## 📊 Dataset Used
**Medical Appointment No Shows** dataset from Kaggle:  
https://www.kaggle.com/datasets/joniarroba/noshowappointments

---

## 🎯 Objective
Clean and prepare the raw dataset to handle:
- Missing values
- Duplicate records
- Inconsistent text formats
- Data type issues
- Date formatting

---

## Tools Used
- Python 
- Pandas 
- Jupyter Notebook / VS Code
- (Optional) Excel for quick inspection

---

## Cleaning Steps Performed

1. **Renamed Columns**  
   Renamed columns to lowercase and replaced spaces with underscores for consistency.

2. **Handled Missing Values**  
   Checked using `.isnull()` – No missing values in this dataset.

3. **Removed Duplicates**  
   Removed exact duplicate rows using `.drop_duplicates()`.

4. **Fixed Invalid Age Entries**  
   Removed rows with age < 0.

5. **Standardized Text Columns**  
   - Gender standardized to uppercase.
   - Neighbourhood names title-cased and stripped of whitespace.
   - No-show column capitalized (`Yes`/`No`).

6. **Converted Binary Columns to Integer**  
   Columns like `scholarship`, `diabetes`, etc. were converted to `int`.

7. **Formatted Dates**  
   - Converted `scheduledday` and `appointmentday` to datetime.
   - Then formatted to `dd-mm-yyyy` for easier interpretation.

8. **Data Types Fixed**  
   - `age` → `int`
   - `gender`, `neighbourhood`, `no_show` → `category`
   - `scheduledday`, `appointmentday` → string (`dd-mm-yyyy` format)

---



## ✅ Summary
This cleaned dataset is now ready for further analysis or modeling. The data types are fixed, formats are consistent, and unnecessary or invalid data has been removed.

