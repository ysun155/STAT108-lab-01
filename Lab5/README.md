By downloading the file listings.csv from Santa Cruz in this
[website](http://insideairbnb.com/get-the-data.html), we create a
dataset as raw\_data/listing.csv. Here’s an description of the
variables:

-   `price`: Cost per night (in U.S. dollars)
-   `neighbourhood`: Santa Cruz county City (Santa Cruz, Capitola,
    Scotts Valley, etc.)
-   `room_type`:
    -   *Entire home/apt* (guests have entire place to themselves)
    -   *Private room* (Guests have private room to sleep, all other
        rooms shared)
    -   *Shared room* (Guests sleep in room shared with others)
-   `number_of_reviews`: Total number of reviews for the listing
-   `reviews_per_month`: The number of reviews per month the listing has
    over the lifetime of the listing.
-   `minimum_nights`: Number of nights required to book rental

After calculating the prices for three nights stay: cost for three
nights + cleaning fee (2% of price per night), we generate two new
variable - `cleaning_fee` and `price_3_nights`. We also created a
simpler verison to categorize neighborhood called `neigh_simp`:
Unincorporated Areas, City of Santa Cruz, City of Capitola, Other.

For the regression analysis, since we only want to include Airbnb
listings that are intended for travel purposes, we filtered the dataset
and only includes `minimum_nights <= 3`. This new dataset can be found
in mod\_data/airbnb.csv.
