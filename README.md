<h2>Prerequisites</h2>
* Python 3.XX
* Selenium

<h2>Input Parameters</h2>

* _phone_number_ - Phone number or email to log in to amazon

* _password_ - Password for amazon account

* _min_filter_ - specify starting price of laptops. E.g. 30000

* _max_filter_ - specify maximum price of laptops. E.g. 50000

<h2>Additional Info</h2>
* Tests are targeted for Amazon India website. Not tested on Amazon.com
* Asserts in method '_verify_prices_' are commented as amazon shows products out of price filter criteria


<h2>Script Flow</h2>
* Go to https://www.google.co.in/
* Search for Amazon
* Prints all entries in search dropdown
* Hit enter
* Search for https://www.amazon.in & clicks it
* Sign in
* Selects category as "Electronics"
* Search for "dell computers"
* Set price filter
* Verify price of all laptops is between given filter
* Print names of products with 5-star rating
* Repeats last two steps on Page 2
* Goes back to page 1
* Select 1st product with 5-star rating
* Open the product
* Click on Add to wishlist button
* Verify for text "One item added to" to verify item was added to wishlist
