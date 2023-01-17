<p></p><h1>EDA (Univariate data analysis)</h1>
<h1>Univariate Analysis</h1>
<p>Univariate analysis is a statistical method that involves the analysis of one variable at a time. It is used to describe the main features of a single variable, such as its mean, median, mode, range, and variance. The goal of univariate analysis is to describe the distribution of the data and to identify any outliers or unusual observations. It is often used as a first step in data analysis, before moving on to more complex methods such as bivariate or multivariate analysis.</p>
<p>Data are two types</p>
<ol>
<li>Numerical</li>
<li>Categorical</li>
</ol>
<p>EDA starts with univariate analysis</p>
<p>Follow the way—-</p>
<ol>
<li>Find categorical data and show</li>
<li>Count plot (its comes under seaborn )</li>
</ol>
<p><code>#countplot import seaborn as sns sns.countplot(df['Survived'])</code></p>
<ol>
<li>One additional thing although this same but you can use pie chart to show all the above value counts in percentage.</li>
</ol>
<p><code>df['Pclass'].value_counts().plot(kind='pie',autopct='%.2f')</code></p>
<p>Numerical column</p>
<p>In Exploratory Data Analysis (EDA), numerical data refers to data that can be measured on a continuous or discrete scale, such as age, income, temperature, and count of items. Numerical data can be further classified into two types: continuous data and discrete data. Continuous data can take on any value within a certain range, such as weight or temperature, while discrete data can only take on certain specific values, such as the number of children in a family.</p>
<p>To analyze numerical data during EDA, various statistical measures can be used such as mean, median, mode, standard deviation, min and max, percentiles, and box plots. Histograms, scatter plots, and density plots can also be used to visualize the distribution of the data. Additionally, correlation and regression analysis can be used to examine the relationships between variables.</p>
<p>It's important to note that outliers and missing data should be handled carefully during EDA as they can greatly impact the results of statistical analysis.</p>
<ol>
<li>Histogram</li>
</ol>
<p>A histogram is a graphical representation of the distribution of numerical data. It is used in Exploratory Data Analysis (EDA) to visualize the frequency distribution of a single variable. The x-axis of a histogram represents the range of values for the variable, and the y-axis represents the frequency of observations within each range.</p>
<p>To create a histogram, the data is first divided into a set of bins, and the number of observations that fall into each bin is represented by the height of a bar. The width of the bars in a histogram represents the range of values in each bin, and the height of the bars represents the frequency of observations in that range.</p>
<p>Histograms are useful in EDA to quickly identify the overall shape of the distribution, such as whether it is symmetric, skewed or multimodal. They can also be used to identify outliers, and to compare the distribution of different subsets of data.</p>
<p>It's important to note that the choice of bin size can greatly impact the appearance of the histogram and the conclusions drawn from it. Therefore, it's recommended to try different bin sizes to see which one best represents the data.</p>
<ol>
<li>Distplot</li>
</ol>
<p>A distplot, short for "distribution plot," is a type of plot that combines a histogram with a probability density function (PDF) or a kernel density estimate (KDE) in order to visualize the distribution of a single variable. It is a function provided by the seaborn library in Python, which is commonly used in Exploratory Data Analysis (EDA).</p>
<p>A distplot allows you to see the overall shape of the distribution, including whether it is symmetric or skewed, and whether it has multiple peaks. It also provides a visual representation of the density of the data, which can help identify areas where there are more or fewer observations. Additionally, it can also display the mean, median and mode of the data.</p>
<p>One advantage of using distplot over a regular histogram is that it can handle non-numerical data, and it can also be used to estimate the underlying probability density function of the data.</p>
<p>It is important to note that the choice of bandwidth of the kernel density estimate can greatly impact the appearance of the distplot and the conclusions drawn from it. Therefore, it's recommended to try different bandwidths to see which one best represents the data.</p>
<ol>
<li>Boxplot</li>
</ol>
<p>A box plot, also known as a box-and-whisker plot, is a graphical representation of the distribution of numerical data in Exploratory Data Analysis (EDA). It is used to summarize the distribution of a single variable by displaying the median, quartiles, minimum and maximum values, and any outliers.</p>
<p>A box plot consists of a box, which represents the interquartile range (IQR) of the data, and "whiskers" that extend from the box to the minimum and maximum values. The box is defined by the first quartile (Q1) and the third quartile (Q3), which represents the middle 50% of the data. The median (Q2) is represented by a line inside the box. Any data point outside the whiskers is considered an outlier.</p>
<p>Box plots are useful in EDA to quickly identify the overall shape of the distribution, such as whether it is symmetric or skewed, and to identify any outliers. They can also be used to compare the distribution of different subsets of data by plotting multiple box plots on the same graph.</p>
<p>It's important to note that box plots can be misleading when the data has extreme outliers or a large number of observations, it's recommended to use other visualization methods such as scatter plots or histograms to complement the analysis.</p>
<p>Skew</p>
<p>Skewness is a measure of the asymmetry of the probability distribution of a real-valued random variable about its mean. In Exploratory Data Analysis (EDA), skewness is used to describe the shape of a distribution of numerical data. A distribution is considered to be symmetric if the data is evenly distributed around the mean, and the mean, median, and mode are all equal. A distribution is considered to be skewed if the data is not evenly distributed around the mean, and the mean, median, and mode are not equal.</p>
<p>There are two types of skewness: positive skewness and negative skewness. A distribution is positively skewed if the tail on the right side of the distribution is longer or fatter than the tail on the left side. This means that there are more values on the left side of the mean and fewer values on the right side of the mean. A distribution is negatively skewed if the tail on the left side of the distribution is longer or fatter than the tail on the right side. This means that there are more values on the right side of the mean and fewer values on the left side of the mean.</p>
<p>In EDA, skewness can be identified by visualizing the data using histograms, box plots, or other distribution plots, and by calculating the skewness value which can be obtained by different statistical formulas.</p>
<p>It's important to note that skewness alone is not always an indicator of a problem in data analysis, but when it is present, it can indicate that the data is not normally distributed and may impact the validity of certain statistical tests or models. Therefore, it's recommended to examine the data carefully when skewness is present and to consider the best way to handle it.</p>
<p>Note➖ You can called the function called skew() if value is 0 then no skewness, negative value means negative skewness and positive value means positive skewness.</p><br /><p></p>
