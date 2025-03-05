"Create a dashboard to investigate the strong correlation between '[Average Age]' and '[Purchasing Power Index]' in the dataset. Include the following elements:

1.  **Primary Visualization: Scatter Plot:**
    *   X-axis: '[Average Age]'
    *   Y-axis: '[Purchasing Power Index]'
    *   Each point represents a country.
    *   Use color or size of the points to represent '[Quality of Life Index]' (e.g., higher quality of life = larger/brighter points).  This helps visualize if the age-purchasing power relationship is consistent across different overall quality of life levels.

2.  **Correlation Display:**
    *   Prominently display the Pearson and Spearman correlation coefficients between '[Average Age]' and '[Purchasing Power Index]'.  Use a card visual or a large text box to make these values easily noticeable.

3.  **Trend Analysis:**
    *   Add a trend line (linear) to the scatter plot. Display the equation of the trend line and the R-squared value to quantify the strength and nature of the linear relationship.  Consider adding a smoothed trend line (e.g., LOESS) as well, to see if there are non-linear patterns.

4.  **Supporting Visualizations (Choose *one or two* that best fit the story):**
    *   **Option A: Grouped Bar Chart:**  Divide the '[Average Age]' into age groups (e.g., "Young," "Middle-Aged," "Old",  you'll need to define the age ranges). Create a bar chart showing the *average* '[Purchasing Power Index]' for each age group.  This provides a simplified view of the relationship.
    *   **Option B:  Conditional Box Plots:**  Create box plots of '[Purchasing Power Index]', but *conditioned* on different '[Average Age]' ranges.  For example, one box plot for countries with '[Average Age]' below a certain value, another for a middle range, and a third for a high range. This shows the *distribution* of purchasing power within different age groups.
    *   **Option C:  Table with Extreme Values:**  Create a table listing the countries with the *highest* and *lowest* '[Average Age]' values. Include their corresponding '[Purchasing Power Index]' and '[Quality of Life Index]' values.  This highlights any outliers or particularly interesting cases.

5.  **Slicers/Filters:**
    *   **Country Slicer:**  Allow users to select individual countries to highlight them on the scatter plot and other visuals.
    *    **Region Slicer** (if available and reliable, *not* the dummy data): Include a slicer for '[Region]' to see if the relationship holds within different geographical areas.  If using the dummy region data, clearly label it as "Placeholder - Requires Accurate Region Data."
    * **Year Slicer** (If available)

6. **Textbox:**
* Use Textbox to indicate which method you used to calculate the correlation, and which method used to draw the trendline.

Dashboard Title:  'Age and Purchasing Power: Exploring the Correlation'
"

# 关键改进说明:

强调年龄: 由于年龄是核心，Prompt 更明确地指导如何围绕年龄构建可视化。

多种趋势分析: 除了线性趋势线，还建议使用平滑曲线 (LOESS) 来捕捉可能的非线性关系。 年龄与购买力之间很可能不是简单的直线关系。

分组/条件可视化: 提供了几种可选的辅助可视化方法，这些方法都将年龄数据分组或分段，以更清晰地展示不同年龄段的购买力情况。

明确的度量: 要求显示趋势线方程和 R 方值，以量化关系。

突显生活质量: 通过颜色/大小编码 [Quality of Life Index]，可以在年龄-购买力关系中看到整体生活质量的影响。

Slicer 的优先级: 将国家筛选器放在更重要的位置，因为查看特定国家的数据通常很有用。

Textbox 说明: 强调使用 Textbox 去解释说明关联性和趋势线。

这个 Prompt 旨在创建一个重点突出、信息丰富的仪表板，深入探索年龄和购买力之间的关系。 它不仅仅是展示相关性，还试图揭示更深层次的模式和潜在的非线性关系。
