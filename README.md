## Background: Mouse Tumor Analysis

  ![Laboratory](Images/Laboratory.jpg)

While my data companions rushed off to jobs in finance and government, I remained adamant that science was the way for me. Staying true to my mission, I've joined Pymaceuticals Inc., a burgeoning pharmaceutical company based out of San Diego. Pymaceuticals specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a data analyst at the company, I've been given access to the complete [data](Pymaceuticals/data/Mouse_metadata.csv) from their most recent animal study. In this study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. I have been tasked by the executive team to generate all of the tables and figures needed for the technical report of the study. The executive team also has asked for a top-level summary of the study results.

I will do the follwing:

* Check the data for any mouse ID with duplicate time points and remove any data associated with that mouse ID.<br>
  ![Duplicate Mouse ID](Images/duplicate_mouse.png)

* Generate a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.<br>
  ![Summary Statistics Table](Images/statistics_table.png)

* Generate a bar plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows  the number of total mice for each treatment regimen throughout the course of the study.<br>
  ![Pandas Treatment Regimen](Images/pandas_drug_regimen_bar.jpg)<br>
  ![Pyplot Treatment Regimen](Images/pyplot_drug_regimen_bar.jpg)

* Generate a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the distribution of female or male mice in the study.<br>
  ![Pandas Gender Distribution](Images/pandas_mouse_sex_pie.jpg)<br>
  ![Pyplot Gender Distribution](Images/pyplot_mouse_sex_pie.jpg)

* Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Calculate the quartiles and IQR and quantitatively determine if there are any potential outliers across all four treatment regimens.<br>
  ![Promising Treatment Outliers](Images/treatment_regimen_outliers.png)

* Using Matplotlib, generate a box and whisker plot of the final tumor volume for all four treatment regimens and highlight any potential outliers in the plot by changing their color and style.<br>
  ![Final Tumor Volume](Images/final_tumor_volume_box.jpg)

* Select a mouse that was treated with Capomulin and generate a line plot of tumor volume vs. time point for that mouse.<br>
  ![Capomulin Treatment Line Plot](Images/tumor_volume_time_point_line.jpg)

* Generate a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen.<br>
  ![Capomulin Treatment Scatter Plot](Images/avg_tumor_vol_mouse_weight_scatter.jpg)

* Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment and plot the linear regression model on top of the previous scatter plot.<br>
  ![Capomulin Treatment Linear Regression](Images/avg_tumor_vol_mouse_weight_regression.jpg)

  - - -

## Written Report

  * Overall, Capomulin is the favored drug regimen to reduce tumor growth.
  * Capomulin had the most number of mice complete the study, with the exception of Remicane. All other regimens observed a number of mouse casualties across the study.
  * There is a strong correlation between mouse weight and tumor volume indicating that mouse weight may be contributing to the effectiveness of any drug regimen.
  * Most mice showed tumor volume increase excluding one outlier mouse that had a reduction in tumor growth in the study using the Infubinol regimen.

  - - - 

## References

Mockaroo, LLC. (2021). Realistic Data Generator. [https://www.mockaroo.com/](https://www.mockaroo.com/)

- - -

Contact Information:
* [LinkedIn](https://www.linkedin.com/in/DConnellyII)
* Darryl.Connelly.II@gmail.com