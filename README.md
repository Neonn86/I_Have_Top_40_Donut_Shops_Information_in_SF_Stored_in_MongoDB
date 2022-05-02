# Scrape & Store SF's Top 40 Donut Shop information in MongoDB
## Objective
The goal is to scrape San Francisco's top 40 donut shop information and store them into MongoDB.

## Data Source
- On yelp.com, use **BeautifulSoup** in **Python** to search for the top-40 “Donut Shop” in the San Francisco area according to Yelp's "Recommended" sorting.
- For each store, scrape the following information:
<img width="700" alt="image" src="https://user-images.githubusercontent.com/98130185/166173160-d2f3d2fd-4f90-4168-afbb-3e0a295d5c03.png">

   - search rank
   - name
   - linked URL [this store’s Yelp URL]
   - star rating
   - number of reviews
   - store tags
   - “$” signs
   - delivery / dine-in tags
   - whether you can order through Yelp


## Structure
- Scrape Store Information.
- Create a **MongoDB** collection called “sf_donut_shops” that stores all the extracted shop information, one document for each shop.
- Scrape each shop’s address, phone number, and website. 
- Sign up for a free account with https://positionstack.com/  =to query each 'shop address’ geolocation (longitude, latitude). 
- Update each shop document on the MongoDB collection “sf_donut_shops” to contain the shop’s address, phone number, website, and geolocation. 
- Place an index on the shop’s search rank. 
