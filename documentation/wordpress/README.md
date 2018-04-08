# Wordpress

To implement the donations in the existing Wordpress install, the WooCommerce plugin was used to create "products" for each of the causes/categories.

A new "donation" product type was defined, with variable price.

The donate buttons on the Donations pages are implemented as a product listing, which link through to the product page

In order to avoid breaking existing bookmarks and links, we used a Redirection plugin to redirect from the program pages to the new product pages.

Some selective CSS overrides customize the presentation of the donation blocks. This CSS is injected using the Custom CSS & JS plugin. The contents of the [custom-css.css](./custom-css.css) should be used.

