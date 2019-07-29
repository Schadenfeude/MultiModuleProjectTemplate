# eC@rt  
An app that allows you to scan products’ barcodes and gives you information about them.
It also allows you to mark your favorite stores on the map so you know where to go to buy
the cheapest and best quality products.

## TODO
 - [x] Change color theme to a lighter one
 - [x] Add MyCart fragment
 - [x] Redirect scan flow to add products to the cart directly
 - [x] Make payment fragment where you choose how you pay
 - [x] Make a store checkout fragment where you get a QR code with your list of bought items
 - [x] Add cart shortcut (FAB) to main fragment
 - [x] Add a QR code generation and update `PaymentFragment` to show a meaningful QR code
 - [x] Import CBA database and query it for products as first source of truth
 - [x] Add only barcodes to the QR code
 - [ ] Update Java code to Kotlin
 - [x] Update model or add new model containing item count
 - [ ] Fix backtracking from `PaymentFragment` to `BarcodeScanFragment`
 - [ ] Add option to favorite products in cart and add favorite products to cart
 - [ ] Tryout the new Android Studio and its new Navigation Editor to make transition animations
 - [x] Research if ZXing can be, and is better to use as a barcode scanner - 
    this might work, but it uses its own Activity so it might be slower and harder to use
 - [ ] Add images in the assets folder and link them to the Products model or use Google images API

## IMPORTANT
To be able to run this app properly, you will need an **API key** for Google Maps and UPC Database. 
 - To create your Google Maps key go to 
 [this page](https://developers.google.com/maps/documentation/embed/get-api-key#detailed-guide) 
 and follow the instructions in the **Detailed Guide to getting an API key** section. 
 - To create your UPC Database key go to [this page](http://upcdatabase.org/signup) and sign up. 
 After you do, log into your account, go to the **API Access** setting (to your left) and create a new
 API token.
 
 After you create your keys open your project's `gradle.properties` file and add the following lines:

 `MapsApiKey = {YOUR_KEY}`
 
 `UpcDbApiKey = {YOUR_KEY}`
 
 #### Note:
 If the products you wish to scan are not in the database you can add them via [this link](http://upcdatabase.org/add).