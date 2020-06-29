# Coding Discussion 07

# Instructions
For this coding discussion, please clean and merge the data located in the `Data` folder. There are four datasets in total: one drawn from the [The Armed Conflict Location & Event Data Project (ACLED)](https://www.acleddata.com/), which contains monthly counts for both violent and non-violent event activity in Africa from 1997 onward; and the rest drawn from the World Bank's data portal: (i) the percentage of GDP growth by country-year, (ii) the estimated number of workers in the labor force by country-year; and (iii) the estimated total population by country-year.

Please clean and merge the data so that the following is true:

- The unit of observation is set at the `country-year`.
- Only observations for `Africa` from `1997` to `2018` are retained.
- Right skewed variables are logged (add a 1 to all variable values being transformed if there are zeros in the data).
- All missing entries are imputed using the variable's country mean (e.g. if the value for variable `X` is missing for `Nigeria` in `2000`, please fill that missing value with the average value of `X` for the entire country time span. That is, don't use the values from other countries when computing the mean).

Once the data is clean, use the `statsmodels` module in `python` to run the following linear regression:

> % GDP Growth = Non-violence + violence + labor force + population

In words, examine if political instability effects a developing country's economic growth, controlling for population and work force.

- Does political instability effect growth?
- If so, does certain types of political instability (violence vs. non-violence) have a greater or lesser effect?
- Are there ways you can think to improve the model (i.e. by lagging the independent variables or introducing an interaction)?

Please interpret your results.

## Submit

Please submit your answer as a Jupyter Notebook in the `Submissions/` folder. Title the notebook with your lastname_firstname_netid (`doe_john_jd568.ipynb`). Be sure to submit a docstring if you write any functions indicating what your function does and all the arguments it takes.  As per usual, please submit your answer to the class repository by Friday 11:59pm deadline.

## Response

Please do not respond to anyone's code until after the Friday deadline. Please submit a response by Sunday 11:59pm. Your response should come in the form of a contribution or edit to someone else's code (not just a comment).

- Is there a way you could potentially improve open the logic they laid out by say making the code more concise or efficient?
- Is there another way you could structure the manipulation so that it played out in less steps?
- Did the person make a mistake when cleaning the data?
