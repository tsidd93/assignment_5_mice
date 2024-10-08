# assignment_5_mice
Assignment 5 of bootcamp


Detailed Analysis of Tumor Volume Across Treatment Regimens
Data Overview
This study analyzes the effects of various drug regimens on tumor volume in mice. The primary goal is to investigate how different treatments affect tumor growth, and to identify any significant relationships between mouse characteristics (such as weight) and tumor volume.

Data Cleaning
We began by combining two datasets: one containing mouse metadata and another with study results. After merging the data, we identified and removed duplicate entries for certain mice to ensure the dataset contained unique records for analysis. Specifically, Mouse ID "g989" was removed due to duplicate entries across multiple timepoints.

Statistical Summary of Tumor Volume
We calculated a variety of summary statistics (mean, median, variance, standard deviation, and standard error of the mean) for the tumor volume across four key drug regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.

The results are as follows:

Drug Regimen	Mean Tumor Volume	Median Tumor Volume	Tumor Volume Variance	Tumor Volume Std. Dev.	Tumor Volume SEM
Capomulin	40.68 mm³	41.56 mm³	24.95	4.99	0.33
Ramicane	40.22 mm³	40.67 mm³	23.48	4.84	0.32
Infubinol	52.88 mm³	51.82 mm³	43.13	6.57	0.49
Ceftamin	52.59 mm³	51.78 mm³	39.29	6.27	0.47
Key Findings:

Capomulin and Ramicane both have lower average tumor volumes and standard deviations compared to Infubinol and Ceftamin, suggesting better tumor reduction.
Infubinol had a single potential outlier in tumor volume (36.32 mm³), indicating an unusual observation for one mouse.
Visualization and Analysis
1. Tumor Volume Distribution
A box plot was generated for each drug regimen, showing the distribution of tumor volumes across mice. The box plot for Capomulin and Ramicane displayed smaller ranges of tumor volumes, indicating these regimens were more consistent in reducing tumor size compared to Infubinol and Ceftamin.

2. Tumor Volume Over Time for Mouse b742 (Capomulin Regimen)
A line plot was created to visualize the tumor volume progression over time for a single mouse treated with Capomulin. This plot clearly shows a reduction in tumor size, illustrating the effectiveness of the treatment over the study period.

3. Mouse Weight vs. Tumor Volume (Capomulin Regimen)
We explored the relationship between mouse weight and average tumor volume for the Capomulin regimen. A scatter plot was generated, showing a strong positive correlation between mouse weight and tumor size (correlation coefficient: 0.84). A linear regression model was fit to the data, with the following equation:

Tumor Volume
=
0.95
×
Weight
+
21.55
Tumor Volume=0.95×Weight+21.55
The high correlation suggests that heavier mice tend to have larger tumors on average, even under the Capomulin treatment.
Conclusion
Capomulin and Ramicane appear to be more effective at reducing tumor size compared to Infubinol and Ceftamin, with lower average tumor volumes and fewer variations in outcomes.
There is a strong correlation between mouse weight and tumor volume for mice treated with Capomulin, suggesting that weight may influence tumor growth or the effectiveness of the treatment.
Further studies could explore why heavier mice tend to have larger tumors, and whether this affects treatment outcomes.
