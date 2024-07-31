# Simple Linear Regression Calculations Using Google Sheets

## Entering Data:

1. Go to Google Sheets and start a new blank spreadsheet.
2. Enter Your Data:
    - Click on cell A1 and type in your first data label like "X Values."
    - Click on cell B1 and type in your second data label like "Y Values."
    - Enter your data points below each label. For example:
        - Column A: X Values (e.g. 1, 2, 3, 4, 5)
        - Column B: Y Values (e.g. 2, 4, 6, 8, 10)

## To Create Your Graph with a Least-Squares (Best-Fit) Line:

### Create a Scatter Plot
1. Select Your Data:
    - Click and drag to select the range of your data. For example, if your data is in cells A2 to B6, select that range.
2. Insert a Chart:
    - Click on the “Insert” menu at the top of the page and select “Chart” from the dropdown menu.
3. Change Chart Type:
    - In the Chart Editor that appears on the right, make sure you are on the “Setup” tab.
    - Change the “Chart Type” to “Scatter Chart” if it’s not already selected.

### Add a Trendline
1. Open Chart Editor:
    - Click on the chart you created to open the Chart Editor on the right side.
2. Customize Chart:
    - Go to the “Customize” tab in the Chart Editor.
3. Add Trendline:
    - Click on “Series” to expand that section.
    - Scroll down and check the box next to “Trendline.”
4. Adjust Trendline:
    - You can choose “Linear” for a simple linear regression.
    - Also, check the box for “Show R2” to see the R2 value.

## Calculate the R Value:
1. Click on a blank cell where you want the r value to show up.
2. Enter the CORREL Formula:
    - In the selected cell, type the formula: `=CORREL(A2:A6, B2:B6)`
    - Be sure to replace `A2:A6` and `B2:B6` with the actual ranges of your data if they are different.
    - After typing the formula, press Enter. The cell will display the r value.