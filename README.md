# SkaterZap 
Skaterzap is a multi language ecommerce website, demonstrating uses of HTML, CSS, Python, Django and Javascript in a website built as a concept to be developed further in collaboration with leaders in the local skate community.

The repository can be found [here](https://github.com/DavidJF97/skaterzap)

### Planning Stage
User stories were developed in google spreadsheets alongside the client.
the link to the spreadsheet is [here](https://docs.google.com/spreadsheets/d/1-BkDylt1X3lK7xru8J0QD0EiVzen7ozluGYMt3gB5g8/edit?usp=sharing)

## Features

* Login/Logout/Register/Profiles
* Shopping cart
* Checkout/Payment system(Stripe)
* Products database
* Product pages + individual product details pages
* Search functionality within the store
* Responsive on all devices
* Easy to use navigation
* Product management capabilities

--------

## Structure

The website should be straight forward to use and simple to understand, it should be intuitive and enjoyable to use, which the structure should represent.

### Home page

    The home page is simple and welcoming, giving the user enough information to begin shopping without overloading them with content.

#### Contents of the home page

    * Hero Photo of a skater 
    * A call to action in the form of reccomending the user visit the store and view the latest deals
    * Button that send the user to the store underneath the call to action
    * Navbar
    * Banner displaying a special free delivery deal to insetivise customers to buy more items

### Store

    The store is easy to navigate, with plenty of search and sort options. This was done by sorting by rating, price and category, the search function sorts by category and product name.

#### Contents of the store page

    * Nav bar
    * Banner displaying a special deal to increase customers desires to buy items
    * Products
    * Sort options
    * Update and delete functionality that only the admin can see

### Product details

    The product details page focuses on the details of the individual product and sell the item to the user. This was done by having a description, a product photo, a rating, category type, a price and add to cart, This is everything a customer should need to make a descision on wether to purchase an item or not.

#### Contents of the product details page

    * Nav bar
    * Banner displaying a special dea lto increase customers desires to buy items
    * Product details(description)
    * Product photo
    * Product rating
    * Category type
    * Product price
    * Add to cart

### Toasts

    The toasts inform the user of any action that the customer makes, such as added an item to the cart, or login and log out of the users account. This was done for adding and removing a product from the cart, purchasing an item, registering an account, loggin in and  out, this also includes warnings and errors with anyhting that may go wrong with the site.

### Profiles

    The profile is made up of 2 parts, a form for the users address and a product history. The address form is to speed up checkout times as when the form is filled out and saved, it will automatically fill in the checkout form in for you, all you need to do is fill in the payment details. The order history is to help the user see what they bought from us before, for example, if they cant remember the parts they bought and need the same parts again, they can visit this section and see waht they ahve bought before.

#### Contents of the profiles page

    * Navbar
    * User address
    * Order history

### Shopping cart and checkout

    The shopping cart is easy to understand, it tells the user what they will buy and how much it will cost, featuring a breakdown of the payment, such as delivery cost and total price for the items.

#### Contents of the Shopping cart page

    * Navbar
    * What the user will buy
    * Continue to payment button 
    * Go back to products button


### Checkout

    The checkout is the same as the shopping cart except with a form for the users address and payment details and also inform the user of what they are buying with a price breakdown in the same way as the shopping cart page.

#### Contents of the Shopping cart page

    * Navbar
    * Delivery form
    * What the user will buy

### Product management

    The product management is a simple to use page for the admin to add, create and delete products without accessing the backend of the website, it features add create and delete options which are clearly marked and has a form featuring everything that the admin will need to set up a product to be sold to the customers.

#### Contents of the Product management page
    * Navbar
    * Product form
    * Save and delete options


## Testing

### Responsiveness

The site was tested to ensure responsiveness on screen sizes from 320px and upwards on Google Chrome, Microsoft Edge and Internet Explorer.

Steps to test:
1. Open browser and navigate to BFGuesthouse
2. Open the developer tools (right click and inspect)
3. Set to responsive
4. Click and drag the responsive window to test different maximum widths

Expected:

Website is responsive on all screen sizes and no images are pixelated or stretched. No elements overlap.

Actual:

Website behaved as expected.

Website was also opened on the following devices and no responsive issues were seen:
Iphone SE, Iphone XR, Ipad Air, Ipad Mini

### Validity
* HTML
    * No errors were returned when passing through the official [W3C validator](https://validator.w3.org/)

* CSS    
    * No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/)

* PEP8
    * No errors were returned from PEP8 testing i Gitpod Terminal.

## Deployment

The site was deployed via [Heroku](https://dashboard.heroku.com/apps)

This project was developed utilising the Code Institute Template. Some of the deployment steps below are specifically required for the new CI template and may not be applicable to older versions, or different projects.

Before deploying to Heroku pip3 freeze > requirements.txt was used to add all imports for deployment.

* Log in to Heroku or create an account if required.

* Then, click the button labelled New from the dashboard in the top right corner and from the drop-down menu select Create New App.

* You must enter a unique app name, (I used mastermind-code-breaker).

* Next, select your region, (I chose Europe as I am in Ireland).

* Click on the Create App button.

* The next page you will see is the project’s Deploy Tab. Click on the Settings Tab and scroll down to Config Vars.

* Click Reveal Config Vars and enter PORT into the Key box and 8000 into the Value box and click the Add button.

* Next, scroll down to the Buildpack section click Add Buildpack select python and click Save Changes.

* Repeat step 8 to add node.js. o Note: The Buildpacks must be in the correct order. If not click and drag them to move into the correct order.

* Scroll to the top of the page and now choose the Deploy tab.

* Select Github as the deployment method.

* Confirm you want to connect to GitHub.

* Search for the repository name and click the connect button.

* Scroll to the bottom of the deploy page and select preferred deployment type:

* Click either Enable Automatic Deploys for automatic deployment when you push updates to Github.

* Select the correct branch for deployment from the drop-down menu and click Deploy Branch for manual deployment.

DISCLAIMER: Despite being successfully deployed, the site is currently displaying a BadRequest404, this will be resolved in future development.
The live link can be found here - https://skaterzap-b923c1e51116.herokuapp.com/