# Bluetooth Beacon

A BLE (Bluetooth Low Energy) Beacon can broadcast a URL to nearby mobile devices. This mechanism is specified and documented as [Eddystone](https://developers.google.com/beacons/) and is implemented in Android as the "Nearby" API. This works without a dedicated app in some modern devices, others will need to have a beacon app installed.

Beacons can be battery or USB powered. The URL they broadcast can be configured using a normal Android phone with the appropriate app, setting the Eddystone-URL field. The max-length on this field is 17 bytes, so most URLs will need to be shortened using a URL shortener service like [bit.ly](http://bit.ly/)

To use the beacon, Bluetooth will need to be enabled on the mobile device. On entering the range of the beacon (this is configurable when programming the beacon), the mobile device will typically pop up a notification announcing the presence of the beacon and display the URL (and in some cases, a card summarizing the contents of the target URL.) Apps like Google's Physical Web will follow redirects to read and display the page title, favicon etc.

Clicking on the notification will open the user's web browser to the Donate page.
