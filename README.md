# Airbnb

Dataset :- https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata

### Data Cleaning 
- Several columns had inconsistent data, including spelling errors, which were corrected using the replace function.
- A particular character in the numerical variable turned it into the meaning of the numerical column.
- More than 90% of the values in missing column values are dropped.

### EDA Summary 
- Twenty hosts made more money, including "Rema," "Esaie," "Ilean," "Antonin," "Chun Kit," "Jeff & TJ," "Denae," "Muneeza," "Gat," "Nahi," "Sunika," "Kethy," "Leojohn," "Céline," "Aidas," "Glenis," "Maximillian," and "Tamara & Fran."
- Top 20 hosts include "Michael," "David," "John," "Alex," "Sonder (NYC)," "Daniel," "Karen," "Sara," "Maria," "Anna," "Chris," "Michelle," "Jessica," "Laura," "Mike," "Blueground," "James," "Melissa," and "Amy."
- Top 20 neighbourhood names include "Bedford-Stuyvesant," "Williamsburg," "Harlem," "Bushwick," "Hell's Kitchen," "East Village," "Midtown," "Crown Heights," "East Harlem," "Chelsea," "Greenpoint," "Lower East Side," "Astoria," "Washington Heights," "Financial District," "West Village," "Flatbush," and "East Flat.
- The top neighbourhood groups in terms of price are Queens, the Bronx, Brooklyn, Staten Island, and Manhattan.
- The neighbourhoods of "Manhattan," "Brooklyn," "Queens," "Bronx," and "Staten Island" have received the most reviews.
- The top five cities are Staten Island, the Bronx, Queens, Manhattan, and Brooklyn.
- The price rises in tandem with the service cost.
- Strong correlations exist between pricing, service fee, quantity of reviews, and reviews per month.

### Feature Engineering
- Replace categorical missing values with mode imputation
- Numerical missing values wih median imputation


#### Outlier treatment observation
- Given that the data is, at best, insufficient, few rows feature values greater than 500. 9.5 was the result of the upper bound for the iqr technique, which is a less inconsistent way to treat an outlier.
- In availability 365 few values are greater than 365.
- While reviews offer additional information about the host and city, removing outliers from the remaining columns, such as "number of reviews," "reviews per month," and "review rating number," may reduce the quality of the data.

### Future work 
- Taking effective care of outliers
- Using the ML algorithm to forecast prices
