# Feedback on Final

Excellent work on your final project.  The notebook was easy to follow and your explanations were clear.

Adding the maps at the end was an Excellent idea. What a great visualization and great approach to creating what you wanted without adding on a lot of extra Python requirements.  You can do some great geospatial analysis with Python, but that was outside the scope of expectations for this course.  Another way to visualize this data would have been to use a heatmap or use the actual ZIP boundary shapes with various shading inside to represent how many drop boxes were in each ZIP or density of drop boxes per capita in the ZIP.

One thing to note on the use of color in your charts - I like the consistency between the bar charts and the map. Consistency is good, but it might be an example of overuse of color.  In the bar charts, the columns themselves with labels at the bottom give you enough information about which ZIP is which - color isn't necessary.  On a map, the location of the ZIP shape would provide you that same information - color isn't necessary.  Then you could use color on the map to denote the metrics you've chosen.

I would have liked to see more modularity in your code.  There were a two transformation functions like `to_upper()` and `replace_values` that are kind of throw-away.  The logic within those functions was already self-explanatory, so they weren't really necessary.  Similarly, your `zip_codes()` function could have been replaced with something simpler to truncat the zip codes.  Perhaps: `df['ZIP'].str[:3] + '00'`.  At first, I was confused about why your ZIP values were all 4 digits (instead of the usual 5), but then I realized they were all New England states, where the first digit is a `0`.  Be careful reading numeric looking codes as a number data type.  (-3 on Modularity / Style for limited use of functions)

* Data Access and Formats (5): 5
* Data Merging (5): 5
* Data Aggregation and Pivoting (5): 5
* Data Transformation (5): 5
* Data Visualization (5): 5
* Problem Applicability (5): 5
* Modularity / Style (15): 12
* Documentation and Processionalism (15): 15
