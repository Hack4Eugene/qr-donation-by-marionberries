# Wordpress

To implement the donations in the existing Wordpress install, the WooCommerce plugin was used to create "products" for each of the causes/categories.

A new "donation" product type was defined, with variable price.

The donate buttons on the Donations pages are implemented as a product listing, which link through to the product page

In order to avoid breaking existing bookmarks and links, we used a Redirection plugin to redirect from the program pages to the new product pages.

Some selective CSS overrides customize the presentation of the donation blocks. This CSS is injected using the Custom CSS & JS plugin. The contents of the [custom-css.css](./custom-css.css) should be used.

# Import/Export

Our working environment consisted of exporting the current Wordpress site using the All-in-one WP Migration plugin then importing the files to a new Wordpress Lightsail instance. 

In order to get the new donations pages and updates we made over the weekend migrated to the old working site, a few things will need to be done.

1.) If a cloud based site is wanted, an AWS account will need to be created to host a Lightsail Instance
2.) Export current test Wordpress admin site and import back to the live Wordpress admin site
3.) Create a non-profit Stripe account to get discounts and live charges running