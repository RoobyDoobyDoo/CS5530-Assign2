A) Look for the missing values in all columns and either impute them or drop them

I had to do this part out of order becuase I wanted to impute the values based on other likely related columns to get better results.

Too many values are missing in 'New_Price' to be useful, I dropped that whole column.

Imputing the rest should be fine. I imputed them using more advanced methods I learned in my Intro to Machine LEarning class.
- Mileage was imputed addtionally using engine size and year.
- I wanted to impute engine size and seat number using model name but didn't want to encode all those names. I opted to just impute on itself.
- Power was imputed from engine size and year. Again, I would've added model name too if it was simple to implement.


B) Also, when I was cleaning up the numerical columns, there were km/kg values thrown in with the kmpl (km/l) data.
I looked online to check the density of the fuel types to make sure I could get to the right units.
However, in my head, the unit conversion tells me I should multiply km/kg with kg/l (density) to get the right units.
But when I go to check them against real world values for the mileage on these cars, it looks like I should be dividing instead?
I don't understnad where I'm going wrong conceptually, but other online sources also say to divide, so I did it that way.
