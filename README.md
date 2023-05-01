Download Link: https://assignmentchef.com/product/solved-bigdata-assignment1-diamond-dataset-main
<br>
The dataset for this assignment contains the prices and other attributes of 50,000 diamonds. Your task is to perform an Exploratory Data Analysis on the dataset. Submit an R Markdown report summarising your findings together with the source code. Check Moodle for deadline. This assignment is part of the continuous assessment and worth <strong>30% </strong>of the module grade.

<h1>1          Dataset</h1>

First download the dataset from Moodle. As the dataset contains 50K records, generating the plots may take a few moments. One way is to start with a small sample and carry out analysis, for example, you can pick 10,000 observations (without replacement) using the function: s<sub>ample</sub>. Run the following code to do so:

s &lt;- sample(nrow(diamonds.dataset), size=10000, replace = FALSE, prob = NULL) diamonds.subset &lt;- diamonds.dataset[s, ]

The above piece of code creates a new dataset named: diamonds.subset containing 10,000 observations from diamond dataset. You can use the sampled dataset (diamonds.subset) first to write and test your code. And then use the full dataset for completing the task given below. REMEMBER! You must report your findings on the <strong>fulldataset</strong>. In your final report, there is no need to include your findings on the sampled dataset. When you load the dataset, you will find the following variables in the dataset: <strong>carat: </strong>weight of diamond (0.2 to 5.01) <strong>cut: </strong>quality of the Cut (Fair, Good, Very Good, Premium) <strong>color: </strong>diamond color from D (Best) to J (Worst)

<strong>clarity: </strong>a measurement of how clear the diamond is from I1 (Worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (Best) <strong>table: </strong>width of top of the diamond

<strong>x: </strong>length in mm <strong>y: </strong>width in mm <strong>z: </strong>depth in mm

<strong>depth: </strong>total depth percentage = 2*z/(x+y) <strong>price: </strong>price in US dollars

<h1>2          Task</h1>

Your task is to perform EDA and calculate the strength of relationships between the variables of the dataset. Consider below as a guideline:

<ol>

 <li>Your first task is to clean the dataset and prepare it for analysis by</li>

</ol>

e.g. removing/replacing NAs and incorrect values. <strong>(20 points)</strong>

<ol start="2">

 <li>Begin your analysis with a summary of the variables (use basic statistical methods). Briefly describe your understanding. Prepare 4 plots: pie chart, bar chart, histogram, scatter plot. Each plot should display different variables (do not use p<sub>rice </sub>variable now). Each plot must have a title and meaningful labels. <strong>(20 points)</strong></li>

 <li>Focus your analysis on the price variable: <strong>(20 points)</strong>

  <ul>

   <li>Show the histogram of the price variable. Describe it briefly. Include summary statistics like mean, median, and variance.</li>

   <li>Group diamonds by some price ranges (like low, medium, high, etc.) and summarise those groups separately.</li>

   <li>Explore prices for different cut types. You might want to use the</li>

  </ul></li>

</ol>

boxplot.

<ul>

 <li>How different attributes are correlated with the price? Which 3 variables are correlated the most with price?</li>

</ul>

<ol start="4">

 <li>Now focus your analysis on the carat, depth, table and dimensions (x, y , z) variables: <strong>(20 points)</strong>

  <ul>

   <li>Compute a volume variable from x, y, z – add it to the dataset.</li>

  </ul></li>

</ol>

Plot it against the price. Describe your findings.

<ul>

 <li>Are the carat and volume attributes correlated? Is that a strong relationship? Draw a plot with regression line.</li>

 <li>Explore the relationships between table and depth variables.</li>

 <li>Now explore relationships between table and rest of other variables. Compute correlations and describe your findings.</li>

</ul>

<ol start="5">

 <li>In your Markdown document, you should use proper headings and commentary for each task. You can get up to <strong>20 points </strong>for style, clarity and quality of the report and the source code.</li>

</ol>

<strong>Keep in mind the following…</strong>

<ul>

 <li>Acceptable file format: Knit your Markdown document in pdf output. Use the submission link on Moodle to upload your final <strong>pdf </strong> In your pdf, you must echo the final version of your code for each task and its output. And add some commentary on your findings. Do not include any random R code blocks that you may write for initial/rough work!</li>

 <li>There will be a late submission penalty as per the College policy. I will be very strict on plagiarism. You may want to read Griffith’s plagiarism policy. I will be awarding ZERO to both the Copyier and Copyee.</li>

</ul>