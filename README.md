
# Lung Cancer Analysis

This project focuses on analyzing lung cancer data using MySQL, Python (with Pandas and Matplotlib), and Jupyter Notebook. The dataset is imported from Excel into a MySQL database, and various visualizations are created to understand and interpret the data.

## Project Structure

### 📂 Data Source
The data used in this project is initially stored in an Excel file. It contains various features such as:
- **🔵 GENDER**: Male (M) or Female (F)
- **🔵 AGE**: Patient age
- **🔵 SMOKING**: Indicator for smoking habits
- **🔵 YELLOW_FINGERS**: Indicator for yellow fingers
- **🔵 ANXIETY**: Indicator for anxiety
- **🔵 PEER_PRESSURE**: Indicator for peer pressure
- **🔵 CHRONIC DISEASE**: Presence of chronic disease
- **🔵 FATIGUE**: Indicator for fatigue
- **🔵 ALLERGY**: Indicator for allergies
- **🔵 WHEEZING**: Indicator for wheezing
- **🔵 ALCOHOL CONSUMING**: Indicator for alcohol consumption
- **🔵 COUGHING**: Indicator for coughing
- **🔵 SHORTNESS OF BREATH**: Indicator for shortness of breath
- **🔵 SWALLOWING DIFFICULTY**: Indicator for swallowing difficulty
- **🔵 CHEST PAIN**: Indicator for chest pain
- **🔵 LUNG_CANCER**: Lung cancer diagnosis (YES/NO)

### 📊 Tools and Technologies
- **📃 MySQL**: For data storage and management
- **💻 Python**: For data processing and visualization
  - **🐼 Pandas**: For handling and manipulating data
  - **📈 Matplotlib**: For creating visualizations
- **🔬 Jupyter Notebook**: For interactive coding and analysis

### 🔍 Steps Involved

1. **⚙️ Data Import**:
   - The Excel dataset is imported into a MySQL database named `lung_cancer`.
   - A table named `cancer` is created to store the data.

2. **🔍 Data Extraction**:
   - Data is fetched from the `cancer` table using Python's `mysql.connector` library.
   - Data is converted into a Pandas DataFrame for further analysis.

3. **⚙️ Data Preprocessing**:
   - The dataset is limited to the first 10 rows for visualization purposes.
   - Indexing is reset to start from 1 for better readability.

4. **🎨 Data Visualization**:
   - **📋 Tabular Representation**:
     - The dataset is displayed in a well-aligned table format using the `tabulate` library.
   - **📊 Bar Chart**:
     - A stacked bar chart visualizing the relationship between age and lung cancer diagnosis.
   - **🥧 Pie Chart**:
     - A pie chart showing the distribution of lung cancer diagnosis (YES/NO).
   - **📊 Gender vs Lung Cancer**:
     - A stacked bar chart comparing gender and lung cancer diagnosis.
   - **📊 Boxplot**:
     - A boxplot showing the distribution of age by lung cancer status.

## 🎨 Visualizations

### 1. 📊 Age vs. Lung Cancer
- A stacked bar chart showing the count of lung cancer diagnoses for different age groups.

### 2. 🥧 Lung Cancer Distribution
- A pie chart displaying the proportion of YES and NO diagnoses for lung cancer.

### 3. 📊 Gender vs. Lung Cancer
- A bar chart visualizing the relationship between gender and lung cancer diagnosis.

### 4. 📊 Age Distribution by Lung Cancer Status (Boxplot)
- This boxplot visualizes the age distribution for lung cancer status (YES/NO):

#### Key Insights from the Boxplot:
- **Median Age**: The median age for lung cancer patients (YES) appears lower than for non-patients (NO).
- **Interquartile Range (IQR)**: The IQR for the "YES" group is much larger, indicating a wider age distribution for lung cancer patients.
- **Outliers**: The "NO" group has an outlier above 65 years, which may represent a few older individuals without lung cancer. The "YES" group has a larger spread from 50 to 75 years, with no extreme outliers.
- **Spread & Distribution**: Lung cancer patients have a much wider age spread (50 to 75 years), while non-patients are mostly concentrated around 60-65 years.

## 🚀 Installation and Setup

1. **🔧 Install Required Libraries**:
   ```bash
   pip install mysql-connector-python pandas matplotlib tabulate
   ```

2. **🛠️ Set Up MySQL Database**:
   - Create a database named `lung_cancer`.
   - Import the Excel file into a table named `cancer` using MySQL Workbench or a similar tool.

3. **🔦 Run the Script**:
   - Open the Jupyter Notebook.
   - Execute the provided script to fetch data, process it, and generate visualizations.

## 📊 Output

- Tabular data representation in the console.
- Multiple visualizations showing insights from the dataset.

## 💡 Key Learnings
- Using MySQL to store and manage data effectively.
- Leveraging Python for data analysis and visualization.
- Creating insightful visualizations to understand complex datasets.

## 🚒 Future Work
- Perform more in-depth statistical analysis of the dataset.
- Use machine learning algorithms to predict lung cancer diagnosis.
- Expand the dataset to include more records for better analysis.

---


