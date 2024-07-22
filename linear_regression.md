# Simple Linear Regression

## Overview

A simple linear regression is a mathematical model that describes the relationship between a dependent and independent variable, in order to figure out if there's a relationship between the two things.  For example, let's say you want to know if there's a connection between how much you study for a test and the grade you get.  Simple linear regression helps us see if there's a straight line that can best predict how one thing (like studying time) changes when another thing (like your test grade) changes.


**Here's how it works:**
1. **Data Collection:** First, you collect data. You ask a bunch of students how much they studied (like 1 hour, 2 hours, etc.) and what grade they got (like 70%, 80%, etc.).
2. **Plotting Points:** You plot these points on a graph where the x-axis (horizontal line) shows how much they studied, and the y-axis (vertical line) shows the grade they got.
3. **Finding the Line:** Simple linear regression draws a straight line through these points (called the least-squares line or best-fit line). This line tries to show the average relationship between studying time and test grade for everyone in your data.
4. **Making Predictions:** Once you have this line, you can use it to make predictions. For example, if someone studied 3 hours, the line can estimate what grade they might get based on where 3 hours falls on the line.
5. **Understanding Relationships:** Finally, by looking at this line, you can understand if there's a clear connection. Does more studying usually mean a higher grade? The line helps us see how strong this relationship might be.  



In science, we use this method to understand how one thing affects another, like studying time affecting test grades. It's like drawing a line that best fits the data points to see the trend and make predictions based on that trend.
  



Here are some things to know when creating or analyzing linear regressions:
* Slope:
* An upward slope indicates a positive association (as one variable gets larger, so does the other)
* A downward slope indicates a negative association (as one variable gets larger, the other gets smaller)
* Calculating the slope can tell us the rate of change between the two variables

## Example

| Hours Studied | Grade Earned |
| ----- | ----- |
| 1 | 60 |
| 2 | 70 |
| 3 | 75 |
| 4 | 80 |
| 5 | 85 |
| 6 | 88 |

## Calculation Procedures

### Plotting

* To Create the Least-Squares (Best-Fit) Line:
   * Find the mean of the independent variable data (plotted on the x axis)
   * Find the mean of the dependent variable data (plotted on the y axis)
   * Plot a point on the graph where the means for the independent and dependent variables meet
   * Use a ruler to draw a line going through the mean point that fits the most other data points

### Graphing Calculator

* Calculating the r Value:
   * Turn on Diagnostics:
      * Choose Catalog (2nd, 0 button) → Scroll down to DiagnosticOn → Hit enter to get it on the screen, then hit enter to turn on Diagnostics; Should say Done
      * Linear regression will now show up when you do the following…
   * Click on Stat → Choose Edit
   * Enter your data into L1 (independent variable) and L2 (dependent variable)
   * Click on Stat → Arrow over to Calc → Choose LinReg (ax+b)
   * X list = L1; Y list = L2; Leave FreqList and Store RegEQ blank
   * Scroll down and Choose Calculate
   * It gives you y = ax + b
      * a = slope  (rate of change)
      * b = y-intercept (starting value for when x = 0)
      * r = how close the points are to the least-squares line
         * Example r = .98  means there is a positive correlation and it is very strong  (most data points are around the best fit line)
      * r2 = how closely are the dependent and independent variables related
         * Ex: r2 = .97 means there is a 97% chance that dependent variable (y) is explained by the independent variable (x); 3% is due to chance

### Google Sheets

### Python

## Interpreting the Results

### r value (correlation coefficient)

   * The r value is a measure of the strength and direction of the linear relationship between the two variables. In the context of the data we plotted (hours studied vs grade earned), the r value tells us how closely the points cluster around the least-squares line.
   * The r value ranges from -1 to 1.
   * If r is close to 1, it indicates a strong positive linear relationship. This means that as hours studied increases, grade earned tends to increase as well, and the points are closely clustered around the regression line going upwards.
   * If r is close to -1, it indicates a strong negative linear relationship. This would mean that as hours studied increases, grade earned tends to decrease, and the points are closely clustered around the regression line going downwards.  
   * If r is close to 0, it indicates a weak or no linear relationship. This means that there's no clear trend in how hours studied relates to grade earned, and the points are scattered randomly around the regression line.

### r^2 value
   * Science also uses r2 Values:
   * r2 tells us how much of the variation in one thing (like test scores) can be explained by another thing (like study time). It shows how much the independent variable is impacting the dependent variable.
   * r2 can range from 0 to 1.
   * An r2 value close to 1 means the line or curve fits the data points very well. This means that changes in one thing (like study time) can reliably predict changes in another thing (like test scores).
   * An r2 value close to 0 means the line or curve doesn't fit the data points well. This suggests that the relationship between the two things might not be strong or predictable based on the data.
   * r2 helps scientists see if their ideas about how things are related (like studying and test scores) match up with what the data actually show. It helps them decide if their conclusions are strong and if they can trust the patterns they see in their experiments.
   * In biology, r2 values as low as 0.50 are acceptable.

### Outliers:
   * Outliers:
   * An outlier in a data set is a data point that differs significantly from other observations in the data. It can be unusually high or low compared to the rest of the data points. Outliers can distort statistical analyses and models if not handled properly.
   * The first thing to do with an outlier is try to determine why it is different from the rest of the points.
   * If outliers are caused by data recording errors or failure to follow experimental protocol, they can be corrected or deleted.
   * If the cause of the outlier cannot be determined, the data point cannot be deleted because it underestimates the variability of the data collection process.

### Uncertainty
   * Uncertainty in Science:
   * Uncertainty is a key part of scientific research and experimentation and is an important component of reporting scientific results.  It is a numerical estimate of the errors in the data, and can come from measurement errors, variability between data sets, limitations of models, or unknown factors.
   * For example, imagine you're trying to measure the height of your friend, but you can't get the exact measurement because they keep moving. So, you measure a few times and find that their height is around 150 cm, but you're not sure if it's exactly 150 cm. That's where confidence intervals come in.
   * What is a Confidence Interval?
   * A confidence interval is like a range of values that we think a measurement or result is likely to be within. It shows us how sure we are about our estimate
   * Example with Height:
   * Let's say you measure your friend's height several times and find that each time it's around 150 cm, but it varies a little each time (like 149 cm, 151 cm, etc.).  With a confidence interval, you might say, "I'm 95% confident that my friend's height is between 148 cm and 152 cm."  This means you're pretty sure (95% sure) that their height falls within this range, even though you can't say exactly 150 cm.
   * Uncertainty and Confidence:
   * The reason we use confidence intervals is to show how certain or uncertain we are about our measurements or findings.  A wider confidence interval means more uncertainty because the range of possible values is larger. A narrower confidence interval means we're more confident because the range is smaller.
   * In Science:
   * Scientists use confidence intervals in experiments and studies to show how reliable their results are. It helps them communicate not just the average result, but also how sure they are about it.  If a confidence interval is very wide, it means there's a lot of variability in the data or uncertainty in the measurement. If it's narrow, there's less uncertainty.

### Caution
   * Correlation is not the same as causation:
   * Correlation simply indicates that two variables tend to vary together, but it doesn't imply that one causes the other to change.
   * Correlation does not specify the direction of the relationship (which variable is influencing the other), whereas causation involves a clear direction where one variable influences the other.
   * Correlation can be influenced by third variables (confounding variables) that affect both variables being studied, making them appear correlated even if they are not directly related.
   * Mistaking correlation for causation can lead to incorrect conclusions and decisions. Just because two things are correlated does not mean that one causes the other.
   * Establishing causation typically requires more rigorous experimental designs or controlled studies that can manipulate variables and establish a clear cause-effect relationship.