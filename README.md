# Healthcare and Patient Data Analytics Dashboard

**Capstone Project – Data Visualization**

**Name:** Erina T. Khan | **Roll No.:** 2601201043 | **BCA (H) AI & DS** | **SECTION - B**

An interactive analysis of patient appointment data (age, gender, blood pressure, heart rate and appointment date) built with Python, Pandas, NumPy, Matplotlib and Plotly.

> **Note:** The dataset is a small, simulated (fictional) set of 20 patient records created for academic purposes. It contains no real patient information.

## Project Files

| File | Description |
|---|---|
| `Healthcare_Patient_Analytics_Capstone.ipynb` | Jupyter / Google Colab notebook with all the code and explanations |
| `Healthcare_Patient_Dashboard.html` | Exported interactive Plotly dashboard (created when the notebook is run) |
| `README.md` | This file |

## Dataset

20 patient records, 7 original columns and 2 helper columns.

| Column | Type | Description |
|---|---|---|
| Patient_ID | Text | Unique patient identifier (P001–P020) |
| Age | Number | Age in years |
| Gender | Category | Male / Female |
| Blood_Pressure | Number | Systolic blood pressure (mmHg) |
| Heart_Rate | Number | Heart rate (beats per minute) |
| Department | Category | Cardiology, General Medicine, Neurology, Orthopedics |
| Appointment_Date | Date | Date of the appointment (Jan–Jun 2026) |
| Age_Group* | Category | 18-30, 31-45, 46-60, 61-80 |
| BP_Category* | Category | Normal (below 120), Elevated (120–139), High (140 and above) |

\* Created in the notebook from the original columns.

## How to Run

1. Open [Google Colab](https://colab.research.google.com) and choose **File → Upload notebook**.
2. Upload `Healthcare_Patient_Analytics_Capstone.ipynb`.
3. Run the cells from top to bottom (**Runtime → Run all**).
4. The dashboard is saved as `Healthcare_Patient_Dashboard.html` and downloads automatically in Colab. Open it in any web browser.

Libraries used: `pandas`, `numpy`, `matplotlib`, `plotly` (all pre-installed in Colab).

## Notebook Structure

| Step | Content |
|---|---|
| 1 | Import libraries and create the dataset |
| 2 | Data inspection using `shape`, `info()`, `describe()` and `value_counts()` |
| 3 | Correlation analysis: correlation matrix, heatmap, scatter plot and histogram |
| 4 | `groupby()` analysis by gender, age group and department |
| 5 | Interactive Plotly dashboard |
| 6 | Export the dashboard as an HTML file |
| 7 | Reflection |

## Dashboard

The dashboard has four charts, arranged by importance (most important at the top-left):

1. **Scatter plot** – Age vs blood pressure, with a trend line and the 140 mmHg high-BP threshold
2. **Grouped bar chart** – Average blood pressure by age group and gender
3. **Histogram** – Distribution of heart rate
4. **Line chart** – Number of appointments per month

Interactive features: hover for exact values, zoom and pan, and click legend items to show or hide a series.

## Key Findings

- Age and blood pressure have a strong positive correlation (about 0.91).
- Heart rate has only a weak relationship with age and blood pressure (about 0.23 and 0.26).
- Patients aged 61 and above average about 144 mmHg, compared with about 110 mmHg for those aged 18–30.
- Male patients averaged about 137 mmHg and female patients about 128 mmHg.
- 15 of the 20 heart rate readings fall between 70 and 79 bpm.
- Appointments peaked in April.

## Limitations

The dataset is simulated and contains only 20 records, so these findings should not be generalized to a real patient population. Correlation does not prove causation.
