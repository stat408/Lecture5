# Lecture 5: EDA


## Read Dataset \#1

``` r
library(tidyverse)
sharks <- read_csv("https://github.com/stat408/Lecture5/raw/master/shark_attacks.csv")
```

``` r
glimpse(sharks)
```

    Rows: 25,614
    Columns: 22
    $ `Case Number...1`        <chr> "2017.06.11", "2017.06.10.b", "2017.06.10.a",…
    $ Date                     <chr> "11-Jun-17", "10-Jun-17", "10-Jun-17", "Repor…
    $ Year                     <dbl> 2017, 2017, 2017, 2017, 2017, 2017, 2017, 201…
    $ Type                     <chr> "Unprovoked", "Unprovoked", "Unprovoked", "Un…
    $ Country                  <chr> "AUSTRALIA", "AUSTRALIA", "USA", "UNITED KING…
    $ Area                     <chr> "Western Australia", "Victoria", "Florida", "…
    $ Location                 <chr> "Point Casuarina, Bunbury", "Flinders, Mornin…
    $ Activity                 <chr> "Body boarding", "Surfing", "Surfing", "Surfi…
    $ Name                     <chr> "Paul Goff", "female", "Bryan Brock", "Rich T…
    $ Sex                      <chr> "M", "F", "M", "M", "M", "F", "F", "M", "M", …
    $ Age                      <chr> "48", NA, "19", "30", NA, "32", "20", NA, "73…
    $ Injury                   <chr> "No injury, board bitten", "No injury, knocke…
    $ `Fatal (Y/N)`            <chr> "N", "N", "N", "N", "N", "N", "N", "N", "N", …
    $ Time                     <chr> "08h30", "15h45", "10h00", NA, NA, "Shortly b…
    $ Species                  <chr> "White shark, 4 m", "7 gill shark", NA, "3m s…
    $ `Investigator or Source` <chr> "WA Today, 6/11/2017", NA, "Daytona Beach New…
    $ pdf                      <chr> "2017.06.11-Goff.pdf", "2017.06.10.b-Flinders…
    $ `href formula`           <chr> "http://sharkattackfile.net/spreadsheets/pdf_…
    $ href                     <chr> "http://sharkattackfile.net/spreadsheets/pdf_…
    $ `Case Number...20`       <chr> "2017.06.11", "2017.06.10.b", "2017.06.10.a",…
    $ `Case Number...21`       <chr> "2017.06.11", "2017.06.10.b", "2017.06.10.a",…
    $ `original order`         <dbl> 6095, 6094, 6093, 6092, 6091, 6090, 6089, 608…

Many of these variables will require additional expertise dealing with
text strings, so we’ll come back to this dataset later in class.

### Activity \#1

Create a figure to show shark attacks by year

### Activity \#2

Create a figure to show shark attacks in the five countries with the
most attacks.

### Activity \#3

Create a figure to show shark attacks by year in the five countries with
the most attacks.

### Activity \#4

Create a [waffle
plot](https://r-charts.com/part-whole/waffle-chart-ggplot2/) to indicate
common activity when a shark attack occurred.

``` r
library(waffle)
```

## Read Dataset \#2

``` r
seattle_in <- read_csv('http://math.montana.edu/ahoegh/teaching/stat408/datasets/SeattleHousing.csv')
glimpse(seattle_in)
```

    Rows: 869
    Columns: 14
    $ price         <dbl> 1350000, 228000, 289000, 720000, 247500, 850830, 890000,…
    $ bedrooms      <dbl> 3, 3, 3, 4, 3, 3, 4, 5, 3, 2, 3, 3, 1, 4, 4, 1, 2, 4, 5,…
    $ bathrooms     <dbl> 2.50, 1.00, 1.75, 2.50, 1.75, 2.50, 1.00, 2.00, 2.50, 1.…
    $ sqft_living   <dbl> 2753, 1190, 1260, 3450, 1960, 2070, 2550, 2260, 1910, 10…
    $ sqft_lot      <dbl> 65005, 9199, 8400, 39683, 15681, 13241, 4000, 12500, 662…
    $ floors        <dbl> 1.0, 1.0, 1.0, 2.0, 1.0, 1.5, 2.0, 1.0, 2.0, 1.0, 1.0, 1…
    $ waterfront    <dbl> 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,…
    $ sqft_above    <dbl> 2165, 1190, 1260, 3450, 1960, 1270, 2370, 1130, 1910, 10…
    $ sqft_basement <dbl> 588, 0, 0, 0, 0, 800, 180, 1130, 0, 0, 580, 570, 0, 0, 0…
    $ zipcode       <dbl> 98070, 98148, 98148, 98010, 98032, 98102, 98109, 98032, …
    $ lat           <dbl> 47.4041, 47.4258, 47.4366, 47.3420, 47.3576, 47.6415, 47…
    $ long          <dbl> -122.451, -122.322, -122.335, -122.025, -122.277, -122.3…
    $ yr_sold       <dbl> 2015, 2014, 2014, 2015, 2015, 2014, 2014, 2014, 2015, 20…
    $ mn_sold       <dbl> 3, 9, 8, 3, 3, 6, 6, 10, 1, 11, 4, 9, 10, 9, 10, 6, 7, 6…

### Activity \#5

Pose a question and create a visualization to explore that question.