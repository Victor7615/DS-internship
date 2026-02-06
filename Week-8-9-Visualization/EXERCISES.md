# Week 8-9 Data Visualization - Exercises & Solutions

## Exercise Set 1: Matplotlib Basics

### Problems

**1.1 Simple Line Plot**
```python
import matplotlib.pyplot as plt
import numpy as np

# TODO: Create line plot:
# - x values: 0 to 10 (use np.linspace)
# - y values: sin(x)
# - Add title "Sine Wave"
# - Label x-axis "X axis"
# - Label y-axis "Y axis"
# - Add legend
# - Save as 'sine_wave.png'

x = np.linspace(0, 10, 100)
y = np.sin(x)
```

**1.2 Multiple Lines**
```python
# TODO: Create plot with:
# - Line 1: y = sin(x) in blue
# - Line 2: y = cos(x) in red
# - Line 3: y = sin(x) + cos(x) in green
# - All on same plot
# - Add legend
# - Add title and labels
# - Add grid
```

**1.3 Scatter Plot**
```python
# TODO: Create scatter plot:
# - Generate random x, y (100 points)
# - Color by z values
# - Size varies with z
# - Add colorbar
# - Add labels
# - Save figure
```

**1.4 Bar Chart**
```python
# TODO: Create bar chart:
# - Categories: ['A', 'B', 'C', 'D', 'E']
# - Values: [10, 24, 36, 20, 15]
# - Color each bar differently
# - Add value labels on bars
# - Add title and labels
# - Rotate x-axis labels
```

---

## Exercise Set 2: Matplotlib Advanced

### Problems

**2.1 Subplots**
```python
# TODO: Create 2x2 subplot layout:
# - Plot 1: Line plot (sin)
# - Plot 2: Scatter (random)
# - Plot 3: Bar chart
# - Plot 4: Histogram (random data)
# - Add titles to each subplot
# - Adjust spacing with tight_layout()
# - Save figure
```

**2.2 Figure Customization**
```python
# TODO: Create customized plot:
# - Custom figure size (12, 6)
# - Custom colors
# - Custom markers (circle, square, triangle)
# - Custom line styles (solid, dashed, dotted)
# - Add annotations
# - Custom axis limits
# - Custom grid
```

**2.3 3D Plot**
```python
from mpl_toolkits.mplot3d import Axes3D

# TODO: Create 3D plot:
# - X: range(0, 10)
# - Y: range(0, 10)
# - Z: sin(X) * cos(Y)
# - Add colormap
# - Rotate view
# - Add labels
```

**2.4 Heatmap**
```python
# TODO: Create heatmap:
# - 5x5 correlation matrix from random data
# - Use imshow()
# - Add colorbar
# - Add text annotations
# - Custom colormap
```

---

## Exercise Set 3: Seaborn Plots

### Problems

**3.1 Distribution Plots**
```python
import seaborn as sns
import pandas as pd

data = np.random.randn(1000)

# TODO: Create plots for one distribution:
# - Histogram with KDE overlay
# - KDE plot
# - Rug plot
# - Compare with different bins
# - Add titles and labels
```

**3.2 Categorical Plots**
```python
# Create sample dataset
df = pd.DataFrame({
    'Category': ['A']*30 + ['B']*35 + ['C']*25,
    'Values': np.random.randn(90)
})

# TODO: Create:
# - Box plot by category
# - Violin plot
# - Strip plot
# - Swarm plot
# - Compare distributions
```

**3.3 Regression Plots**
```python
# TODO: Create scatter with regression line:
# - Use random correlated x, y
# - Overlay regression line
# - Add confidence interval
# - Customize colors
# - Add labels
```

**3.4 Heatmap**
```python
# TODO: Create correlation heatmap:
# - Generate random data with 5 columns
# - Calculate correlation matrix
# - Create heatmap
# - Annotate with values
# - Use diverging colormap
# - Customize figure size
```

**3.5 Pair Plot**
```python
# TODO: Create pairplot:
# - Use Iris-like dataset
# - Show relationships between variables
# - Color by category
# - Customize palette
# - Diagonal: histogram vs KDE
```

---

## Exercise Set 4: Plotly Interactive

### Problems

**4.1 Interactive Scatter**
```python
import plotly.express as px

# TODO: Create interactive scatter:
# - Random x, y, z data
# - Size by one variable
# - Color by another
# - Hover information
# - Zoom/pan capability
# - Export to HTML
```

**4.2 Interactive Line Plot**
```python
# TODO: Create time series plot:
# - X: dates over 30 days
# - Y: random walk values
# - Add range slider
# - Range buttons (1w, 1m, all)
# - Hover information
# - Add title and labels
```

**4.3 Interactive Bar Chart**
```python
# TODO: Create interactive bar:
# - Categories on x-axis
# - Values on y-axis
# - Colors by category
# - Hover shows values
# - Click legend to hide/show
# - Download as PNG
```

**4.4 Subplots with Plotly**
```python
import plotly.subplots

# TODO: Create 2x2 subplots:
# - Plot 1: Scatter
# - Plot 2: Line
# - Plot 3: Bar
# - Plot 4: Histogram
# - Share x-axis where appropriate
# - Add titles
```

---

## Exercise Set 5: Geographical Visualization

### Problems

**5.1 Choropleth Map**
```python
# TODO: Create choropleth:
# - US state data
# - Color by values
# - Add hover information
# - Custom colorscale
# - Add title
# - Interactive features

# Note: Use provided data or find state-level data
```

**5.2 Scatter Map**
```python
# TODO: Create map with scatter:
# - Latitude/Longitude data
# - Size and color by values
# - Add markers
# - Hover shows information
# - Zoom to region
```

---

## Challenge Projects

### Project 1: Sales Dashboard

**Objective:** Create multi-plot sales visualization

**Requirements:**
```python
# Create sample sales data with:
# - Date, Product, Region, Amount, Profit columns

# TODO: Create dashboard with:
# 1. Time series: Total sales over time (line)
# 2. Product breakdown: Sales by product (bar)
# 3. Regional heatmap: Sales by product x region
# 4. Top customers: Customer name vs amount (horizontal bar)
# 5. Profit margin: Scatter plot (sales vs profit)
# 6. Summary statistics: Text or table

# Requirements:
# - Use subplots
# - Professional styling
# - Clear labels and titles
# - Color-coded by category
# - Save as high-resolution image
```

### Project 2: Statistical Visualization

**Objective:** Visualize statistical concepts

**Requirements:**
```python
# Generate data with different distributions

# TODO: Create visualization showing:
# 1. Distribution comparison
#    - Histogram for each
#    - KDE overlay
#    - Side-by-side or overlaid
# 2. Correlation heatmap
#    - Multiple variables
#    - Annotated values
# 3. Outlier detection
#    - Box plots
#    - Identify outliers
# 4. Group comparison
#    - Violin or box plots
#    - Multiple groups
# 5. Summary statistics table
#    - Mean, median, std for each

# Style professionally
# Add interpretations
```

### Project 3: Data Story Visualization

**Objective:** Tell story with visualization

**Requirements:**
```python
# Choose a topic and dataset
# Examples:
# - COVID-19 cases over time
# - Climate change trends
# - Stock market performance
# - Population statistics

# TODO: Create 5-7 related plots that:
# 1. Show overall trends
# 2. Reveal patterns
# 3. Compare groups
# 4. Highlight outliers
# 5. Support conclusions

# Arrange as dashboard with:
# - Narrative flow
# - Clear titles
# - Consistent styling
# - Annotations
# - Key insights highlighted

# Add text summary of findings
```

---

## Best Practices Exercises

**BP 1: Color Theory**
```python
# TODO: Create plots comparing:
# - Colorblind-friendly vs. problematic palettes
# - Sequential vs. categorical colors
# - Good vs. bad contrast
# - Professional vs. garish styles

# Show each with same data
# Explain why some are better
```

**BP 2: Clarity Comparison**
```python
# TODO: Create same data visualized:
# Version 1: Good practice
#   - Clear title
#   - Labeled axes
#   - Legend
#   - Grid
#   - Appropriate colors

# Version 2: Poor practice
#   - No title
#   - Missing labels
#   - Confusing colors
#   - Too much decoration

# Show side-by-side
# Discuss differences
```

**BP 3: Design Iteration**
```python
# TODO: Take one plot and create:
# Version 1: Basic matplotlib
# Version 2: Styled with seaborn
# Version 3: Interactive with plotly

# Compare ease of use
# Compare clarity
# Compare interactivity
```

---

## Solution Hints

### Matplotlib
- `plt.figure()` for new figure
- `plt.plot()`, `plt.scatter()`, `plt.bar()`
- `plt.xlabel()`, `plt.ylabel()`, `plt.title()`
- `plt.legend()`, `plt.grid()`
- `plt.subplots()` for multiple plots

### Seaborn
- `sns.set_style()` for style
- `sns.scatterplot()`, `sns.lineplot()`
- `sns.boxplot()`, `sns.violinplot()`
- `sns.heatmap()`, `sns.pairplot()`
- Uses DataFrames with column names

### Plotly
- `px.scatter()`, `px.line()`, `px.bar()`
- Built-in interactivity
- `.add_traces()` for multiple plots
- `.update_layout()` for customization
- `.write_html()` to save

---

## Review Checklist

- [ ] All basic matplotlib exercises done
- [ ] Comfortable with subplots
- [ ] Seaborn plots created
- [ ] Plotly interactivity explored
- [ ] Geographical maps attempted
- [ ] 3 challenge projects completed
- [ ] Best practices understood
- [ ] Professional visualizations created
- [ ] Ready for Week 10 (ML)

Excellent visualization skills! You can now tell stories with data! 📊✨
