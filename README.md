# 🍔 Food Delivery Business Analytics

A Python-based **Business Analytics and Data Visualization** project that explores food delivery operations through statistical analysis and visualizations. The project investigates delivery duration, distance, order type, traffic, weather, vehicle type, and delivery-person ratings to support data-driven business understanding.

## Project Objectives

- Summarize delivery times using descriptive statistics.
- Explore the relationship between delivery distance and delivery duration.
- Compare delivery times across order types.
- Investigate delivery times under different traffic conditions.
- Compare delivery durations across weather conditions.
- Explore delivery performance across vehicle types.
- Examine the association between delivery-person ratings and delivery time.
- Communicate findings through visualizations and business-oriented observations.

## Dataset

The project uses `foodtimedataset.xlsx`, an Excel dataset reported to contain approximately **10,001 records and 17 columns before cleaning**.

| Attribute | Description |
|---|---|
| `ID` | Delivery record identifier |
| `Delivery Person ID` | Delivery personnel identifier |
| `Delivery Person Age` | Age of delivery personnel |
| `Delivery Person Ratings` | Delivery-person rating |
| `Restaurant Latitude` | Restaurant latitude |
| `Restaurant Longitude` | Restaurant longitude |
| `Delivery Location Latitude` | Destination latitude |
| `Delivery Location Longitude` | Destination longitude |
| `Order Type` | Type of food order |
| `Vehicle Type` | Vehicle used for delivery |
| `Temperature` | Recorded temperature |
| `Humidity` | Recorded humidity |
| `Precipitation` | Recorded precipitation |
| `Weather Description` | Recorded weather conditions |
| `Traffic Level` | Recorded traffic conditions |
| `Distance` | Delivery distance |
| `Delivery Time` | Delivery duration |

**Data note:** Confirm the units for `Distance` and `Delivery Time`, and the dataset's collection methodology, before interpreting values or making operational recommendations.

## Data Cleaning

The described workflow includes data-quality checks and cleaning steps such as:

- Checking missing values and duplicate records.
- Checking duplicate delivery IDs.
- Removing completely empty rows and exact duplicate rows.
- Removing records without a delivery ID.
- Filling missing numerical feature values with the median.
- Replacing missing categorical values with `Unknown`.
- Retaining missing distance and delivery-time values for analysis-specific filtering.
- Storing the cleaned data in a separate DataFrame (`df_clean`) to preserve the original DataFrame.

Review the notebook to confirm the exact implementation and any analysis-specific filtering.

## Statistical Analysis

Descriptive statistics and summary measures may include:

- Mean and median
- Standard deviation
- Minimum and maximum
- Quartiles
- Average and median delivery time
- Average delivery distance
- Average delivery-person rating

## Visualizations and Questions Explored

1. **Delivery time distribution** — How are recorded delivery durations distributed?
2. **Order type analysis** — How do average delivery times differ across order types?
3. **Traffic analysis** — How do delivery times vary across traffic categories?
4. **Weather analysis** — Which weather categories are associated with different delivery durations?
5. **Distance vs. delivery time** — Is distance associated with delivery duration? A scatter plot, trend line, and correlation coefficient can help explore this.
6. **Vehicle type analysis** — How do delivery durations compare across vehicle categories?
7. **Ratings analysis** — Is there an observable association between delivery-person ratings and delivery duration?

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Google Colab (optional development environment)
- OpenPyXL (Excel file support)

## Repository Structure

```text
food-delivery-business-analytics/
├── Food_Delivery_Business_Analytics.ipynb
├── foodtimedataset.xlsx
├── README.md
├── requirements.txt
└── .gitignore
```

If your actual notebook or dataset has a different filename, either rename it to match this structure or update the relevant paths in the notebook and this README.

## Getting Started

### Option 1: Google Colab

1. Upload `Food_Delivery_Business_Analytics.ipynb` to Google Colab.
2. Upload `foodtimedataset.xlsx` when prompted, or update the notebook's dataset path.
3. Run the notebook cells in order.
4. Review the statistical summaries, charts, and findings.
5. Run any export cells to generate result files, if included in the notebook.

### Option 2: Run Locally

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/food-delivery-business-analytics.git
cd food-delivery-business-analytics
```

Create and activate a virtual environment (recommended), then install the dependencies:

```bash
python -m venv .venv
```

Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter:

```bash
jupyter notebook
```

Open `Food_Delivery_Business_Analytics.ipynb` and run the cells in order. Ensure that the Excel dataset is in the path expected by the notebook.

## Results and Business Insights

Use the notebook's actual output to document findings such as differences in average delivery time across traffic, weather, order, and vehicle categories, as well as the distance–duration relationship.

**Results are intentionally not stated here:** add numerical findings only after checking the executed notebook. Associations and correlations do not establish causation.

## Limitations

- Analysis depends on the completeness and quality of the supplied dataset.
- Different analyses may use different subsets if values are missing.
- Measurement units and data-collection methodology should be verified.
- Observed relationships do not prove that one factor causes a change in delivery time.
- Findings from this dataset may not generalize to all food-delivery businesses or locations.

## Future Enhancements

- Build an interactive dashboard with Streamlit.
- Explore delivery-time prediction using machine learning.
- Add geographical analysis using restaurant and delivery coordinates.
- Conduct statistical hypothesis tests.
- Add time-of-day or peak-hour analysis if timestamp data is available.
- Generate automated business reports.

## Project Information

- **Project:** Food Delivery Business Analytics
- **Domain:** Business Analytics and Data Visualization
- **Type:** B.Tech mini project
- **Language:** Python

## Authors

- **Nilesh Makwana**
- **Kartik Solanki**

B.Tech — Artificial Intelligence & Data Science

## Acknowledgment

This project demonstrates how Python-based statistical analysis and data visualization can be applied to food-delivery data to explore operational questions and communicate data-driven observations.
