# Week 8-9: Data Visualization & Communication

## Overview
Data visualization is how you tell stories with data. These two weeks cover creating compelling visualizations using Matplotlib, Seaborn, and Plotly that help stakeholders understand insights quickly and clearly.

## Learning Objectives
By the end of these weeks, you should be able to:
- [ ] Create professional plots with Matplotlib
- [ ] Design statistical visualizations with Seaborn
- [ ] Build interactive visualizations with Plotly
- [ ] Create geographical visualizations
- [ ] Choose appropriate plot types for data
- [ ] Design effective dashboards
- [ ] Communicate insights visually
- [ ] Apply design principles to visualizations

## Weekly Schedule

### Week 8: Matplotlib & Seaborn Fundamentals

**Monday - Matplotlib Basics**
- Study: Figure and Axes concepts
- Study: Creating basic plots (line, scatter, bar)
- Study: Customization (labels, titles, legends)
- Practice: Basic plotting exercises
- Time: 3 hours

**Tuesday - Matplotlib Advanced**
- Study: Subplots and multi-plot figures
- Study: Colors, markers, and line styles
- Study: Saving figures and file formats
- Practice: Advanced plotting exercises
- Time: 3 hours

**Wednesday - Seaborn Fundamentals**
- Study: Seaborn vs Matplotlib
- Study: Distribution plots (histplot, kdeplot)
- Study: Categorical plots (barplot, boxplot)
- Practice: Seaborn exercises
- Time: 3 hours

**Thursday - Seaborn Advanced**
- Study: Regression plots
- Study: Matrix plots (heatmap)
- Study: Figure-level functions and FacetGrid
- Practice: Complex Seaborn plots
- Time: 3 hours

**Friday - Integration & Project**
- Review Week 8 concepts
- Complete visualization project
- Prepare for Week 9
- Time: 2 hours

### Week 9: Interactive Visualization & Communication

**Monday - Plotly Basics**
- Study: Plotly express for quick plots
- Study: Interactive features (hover, zoom)
- Study: Customization and styling
- Practice: Plotly exercises
- Time: 3 hours

**Tuesday - Advanced Plotly**
- Study: Plotly graph objects
- Study: Subplots with Plotly
- Study: Dashboards with Dash
- Practice: Advanced Plotly
- Time: 3 hours

**Wednesday - Geographical Visualization**
- Study: Choropleth maps
- Study: Scatter maps and bubble maps
- Study: Map styling and customization
- Practice: Geographical plotting
- Time: 3 hours

**Thursday - Visualization Best Practices**
- Study: Color theory and accessibility
- Study: Storytelling with data
- Study: Dashboard design principles
- Practice: Design exercises
- Time: 3 hours

**Friday - Comprehensive Visualization Project**
- Create multi-plot dashboard
- Demonstrate all visualization techniques
- Present findings visually
- Time: 2 hours

## Key Concepts to Master

### Matplotlib Basics
```python
import matplotlib.pyplot as plt
import numpy as np

# Simple plot
x = np.linspace(0, 10, 100)
y = np.sin(x)
plt.plot(x, y)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Sine Wave')
plt.show()

# Figure and axes
fig, ax = plt.subplots(figsize=(10, 6))
ax.plot(x, y)
ax.set_title('Sine Wave')
plt.tight_layout()
plt.show()
```

### Seaborn Plots
```python
import seaborn as sns
import pandas as pd

# Distribution plot
sns.histplot(data=df, x='column', kde=True)

# Categorical plot
sns.boxplot(data=df, x='category', y='value')

# Heatmap
sns.heatmap(df.corr(), annot=True, cmap='coolwarm')

# Regression plot
sns.regplot(data=df, x='x_col', y='y_col')
```

### Plotly Interactive Plots
```python
import plotly.express as px

# Quick interactive plot
fig = px.scatter(df, x='x_col', y='y_col', 
                 color='category', size='size_col')
fig.show()

# With customization
fig = px.line(df, x='date', y='value',
              title='Time Series Plot')
fig.update_layout(hovermode='x unified')
fig.show()
```

## Study Materials

### Primary Resources - Week 8
1. `05-Data-Visualization-with-Matplotlib/01-Matplotlib Concepts Lecture.ipynb`
2. `05-Data-Visualization-with-Matplotlib/02-Matplotlib Exercises.ipynb`
3. `05-Data-Visualization-with-Matplotlib/03-Matplotlib Exercises - Solutions.ipynb`
4. `05-Data-Visualization-with-Matplotlib/04-Advanced Matplotlib Concepts.ipynb`
5. `06-Data-Visualization-with-Seaborn/01-Distribution Plots.ipynb`
6. `06-Data-Visualization-with-Seaborn/02-Categorical Plots.ipynb`
7. `06-Data-Visualization-with-Seaborn/03-Matrix Plots.ipynb`
8. `06-Data-Visualization-with-Seaborn/04-Grids.ipynb`
9. `06-Data-Visualization-with-Seaborn/05-Regression Plots.ipynb`
10. `06-Data-Visualization-with-Seaborn/06-Style and Color.ipynb`

### Primary Resources - Week 9
1. `06-Data-Visualization-with-Seaborn/07-Seaborn Exercises.ipynb`
2. `06-Data-Visualization-with-Seaborn/08-Seaborn Exercises - Solutions.ipynb`
3. `07-Pandas-Built-in-Data-Viz/01-Pandas Built-in Data Visualization.ipynb`
4. `08-Plotly-and-Cufflinks/01-Plotly and Cufflinks.ipynb`
5. `09-Geographical-Plotting/01-Choropleth Maps.ipynb`
6. `09-Geographical-Plotting/02-Choropleth Maps Exercise.ipynb`

## Daily Practice Routine

```
Morning (1.5 hours):
- Review visualization principles
- Sketch plot designs

Active Study (2.5 hours):
- Read plotting examples
- Create plots along with notebook
- Modify examples

Afternoon (1.5-2 hours):
- Complete exercises
- Experiment with datasets
- Create novel visualizations

Evening (30 min):
- Document learnings
- Collect good examples
- Plan next day
```

## Exercises to Complete

### Exercise 1: Matplotlib Fundamentals
- [ ] Create line, scatter, and bar plots
- [ ] Add labels, titles, and legends
- [ ] Create subplots
- [ ] Customize colors and markers
- [ ] Save figures in different formats

### Exercise 2: Matplotlib Advanced
- [ ] Create complex multi-plot layouts
- [ ] Apply color maps
- [ ] Create 3D plots
- [ ] Customize axes and spines
- [ ] Create annotated plots

### Exercise 3: Seaborn Distributions
- [ ] Create histograms and KDE plots
- [ ] Combine multiple distributions
- [ ] Use facet grids
- [ ] Customize distribution plots
- [ ] Analyze data distributions

### Exercise 4: Seaborn Categorical
- [ ] Create box plots, violin plots
- [ ] Make strip and swarm plots
- [ ] Create bar plots
- [ ] Use categorical faceting
- [ ] Compare groups

### Exercise 5: Seaborn Advanced
- [ ] Create heatmaps
- [ ] Make regression plots
- [ ] Use pairplot for relationships
- [ ] Create clusterplots
- [ ] Design custom palettes

### Exercise 6: Interactive Plotting
- [ ] Create Plotly scatter plots
- [ ] Make line and bar charts
- [ ] Add interactive elements
- [ ] Build simple dashboards
- [ ] Create geographical plots

## Challenge Projects

### Project 1: Sales Dashboard
Create a multi-plot dashboard with:
- [ ] Time series of sales
- [ ] Product category breakdown
- [ ] Regional performance heatmap
- [ ] Top customers bar chart
- [ ] Profit margin scatter plot

### Project 2: Statistical Analysis Visualization
Visualize statistical concepts:
- [ ] Distribution analysis with multiple plots
- [ ] Correlation heatmap
- [ ] Outlier visualization
- [ ] Group comparisons
- [ ] Trend analysis

### Project 3: Story with Data
Tell a story using data:
- [ ] Find interesting dataset
- [ ] Create 5-7 related visualizations
- [ ] Arrange as a dashboard
- [ ] Add narrative context
- [ ] Present findings

## Plot Selection Guide

| Data Type | Question | Best Plot |
|-----------|----------|-----------|
| Single Variable | Distribution? | Histogram, KDE |
| Two Variables | Relationship? | Scatter, Regression |
| Two Variables | Comparison? | Box, Violin, Strip |
| Categorical | Counts? | Bar chart |
| Time Series | Trend? | Line plot |
| Correlation | Relationships? | Heatmap, Pairplot |
| Geographical | Location? | Choropleth, Scatter Map |

## Design Principles

### Color
- Use colorblind-friendly palettes
- Avoid rainbow colors for continuous data
- Use sequential for ordered data
- Use diverging for data with midpoint

### Layout
- Remove chart junk (unnecessary elements)
- Use whitespace effectively
- Align elements carefully
- Maintain consistency

### Labels
- Clear, descriptive titles
- Labeled axes with units
- Legend when needed
- Annotations for key points

```python
# GOOD visualization example
fig, ax = plt.subplots(figsize=(12, 6))
ax.scatter(df['x'], df['y'], alpha=0.6, s=100)
ax.set_xlabel('Variable X (units)', fontsize=12)
ax.set_ylabel('Variable Y (units)', fontsize=12)
ax.set_title('Relationship between X and Y', 
             fontsize=14, fontweight='bold')
ax.grid(True, alpha=0.3)
plt.tight_layout()
```

## Common Mistakes to Avoid

1. **Too Many Colors** - Keep palette simple
2. **3D Plots** - Usually harder to read than 2D
3. **Pie Charts** - Use bar charts instead (easier to compare)
4. **Dual Y-Axes** - Can mislead viewers
5. **Missing Labels** - Always label axes and title
6. **Small Fonts** - Make text readable
7. **Overplotting** - Use alpha, size, or facets

## Resources

### Documentation
- Matplotlib: https://matplotlib.org/stable/contents.html
- Seaborn: https://seaborn.pydata.org/
- Plotly: https://plotly.com/python/
- Dash: https://dash.plotly.com/

### Design Inspiration
- Data Viz Project: https://datavizproject.com/
- Observable: https://observablehq.com/@d3/gallery
- Tableau Gallery: https://www.tableau.com/en-us/about/blog/2020/8/best-visualizations-datasets

### Tools
- Color Brewer: https://colorbrewer2.org/
- Coolors: https://coolors.co/
- Font Pair: https://www.fontpair.co/

## Checklist Before Moving to Week 10

- [ ] Completed all Matplotlib exercises
- [ ] Completed all Seaborn exercises
- [ ] Familiar with Plotly basics
- [ ] Tried geographical visualization
- [ ] Completed 3 challenge projects
- [ ] Understand when to use each plot type
- [ ] Can create professional-looking plots
- [ ] Understand design principles

## Tips for Success

1. **Plot Often** - Use visualization to explore data
2. **Iterate** - Create multiple versions, choose best
3. **Get Feedback** - Show others your plots
4. **Study Examples** - Learn from visualization masters
5. **Keep It Simple** - Don't over-complicate plots
6. **Label Everything** - Clarity is key
7. **Tell a Story** - Plots should support narrative

## Common Customizations Reference

```python
# Seaborn style
sns.set_style("whitegrid")  # darkgrid, white, dark, ticks

# Matplotlib figure size
plt.figure(figsize=(12, 6))

# Colors
colors = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728']
ax.plot(x, y, color=colors[0])

# Transparency
ax.scatter(x, y, alpha=0.6)

# Font sizes
ax.set_title('Title', fontsize=16)
ax.set_xlabel('X', fontsize=12)

# Save high quality
plt.savefig('plot.png', dpi=300, bbox_inches='tight')
```

## Next Steps

After visualization, you're ready for:
- **Week 10-12**: Machine Learning & Capstone Project
- You'll visualize model results and insights

Excellent work on creating impactful visualizations! 🎨📊
