# Climate Analysis
This is a work in progress.
Last updated 16 Apr 2024

## Project Overview
Using Python & associated ML libraries to process, visualize environmental data, and subsequently predict trends.

## Technical Highlights
- Data preprocessing with Python and Pandas
- Time series analysis
- Visualization with Matplotlib

## Reflections and Learning Outcomes

Data has been obtained from data.gov.sg. Datasets obtained are split into 3 groups: Energy, Pollution and Temperature.

-Pre-processing
Initially, I developed a script that efficiently processed and visualized data from a single document. However, as the scope of my project expanded to include six additional datasets, I quickly recognized the inefficiency of duplicating the same code repeatedly. This realization prompted me to redesign my approach by developing a robust function that could automate the preprocessing and visualization tasks across multiple files. This would prompt me to shift my strategy entirely, and though challenges were encountered, it also streamlined my workflow and enhanced the scalability of my project, allowing for more seamless integration of additional data while minimizing manual adjustments.

To go into specifics of what I learnt: I learned to create reusable functions for data preprocessing, enabling me to handle multiple files with varying date formats. I overcame challenges such as case sensitivity and data type discrepancies, which taught me the importance of thorough data inspection and consistent preprocessing. I realized the power of dynamic date parsing as I navigated the complexities of processing multiple files with varying date formats. By adapting my function to handle date columns and formats as parameters, I was able to flexibly parse both monthly and yearly data.
I honed my skills in creating reusable functions for data preprocessing, particularly my preprocess_data function, which became a cornerstone of my workflow. 

I encountered the nuances of case sensitivity within column names across different files. My solution was to standardize all column names to lowercase, ensuring consistent access and avoiding potential mismatches.

For time series data, I deliberated on the best approach to indexing. I decided on converting yearly data to year integers for the index and monthly data to PeriodIndex or DateTimeIndex, depending on the plotting requirements.

When it came to visualization, Matplotlib’s requirements for numeric or date-type values on the x-axis taught me the importance of converting PeriodIndex to DateTimeIndex for a successful plot. The process of dynamically selecting the appropriate column for plotting became essential in handling datasets with varying structures. I leveraged loops to scale this process across multiple files, which significantly improved the efficiency of my work.

I learned valuable lessons from each error I encountered. KeyError and TypeError forced me to delve into the sensitivities of data types in Pandas and Matplotlib, such as plotting Period types directly. These experiences reinforced the importance of consistency in data processing and the utility of iterative approaches.

List and dictionary comprehensions not only optimized my code but also deepened my understanding of Python’s capabilities. Debugging each issue was an enlightening experience that taught me the significance of reflecting on every step of the process.

In terms of best practices, standardizing column names during preprocessing emerged as a critical step to avoid issues in the later stages of analysis. Regularly inspecting the structure and types of data in my DataFrames became a part of my routine checks.

Documentation was a key aspect that supported my progress. By meticulously recording each change and the rationale behind it, I built a comprehensive log that will be invaluable for future reference. Additionally, I became more proficient in using version control with Git, which proved essential for managing my code effectively.

This project was a substantial growth opportunity for me. It was a practical exercise in developing robust data processing pipelines and has equipped me with insights and strategies that will be applicable in all my future data analysis endeavors.

## Usage
instructions will be provided at a later date

## Contributions
feel free to offer tips or advice on how this program can be improved