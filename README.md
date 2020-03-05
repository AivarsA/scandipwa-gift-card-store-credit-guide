# ScandiPWA - Gift Card and Store Credit setup guide

#### 1. Verify that Magento Enterprise edition is installed instead of Community Edition

#### 2. Pull locally these pull requests (to be able to add to cart/wishlist gift card products and all related frontend functionality/styling related to gift cards and store credits) - 
https://github.com/scandipwa/quote-graphql/pull/25

https://github.com/scandipwa/wishlist-graphql/pull/7

https://github.com/scandipwa/base-theme/pull/554

#### 3. Clone locally these 2 (contains functionality to add/remove gift cards and/or store credits from cart) -
https://github.com/AivarsA/customer-balance-graphql

https://github.com/AivarsA/gift-card-graphql

#### 4. Run setup:upgrade. Re-create containers with "--force-recreate" if necessary


## Create Gift Card Product
#### Login in admin - Catalog - Products - press on arrow next to Add Product - choose Gift Card
- Enter gift card name, sku and then scroll till "Amount" and enter your desired amounts for gift card
- Or if you want to allow user to choose amount from-to then change "Allow Open Amount" to enabled and enter amount from and amount to values (by enabling allow open amount will ignore "hardcoded" values)
- Add images for product etc.
- Save product

#### Stores - Configuration - Sales - Gift Cards
- For testing purposes change "Generate Gift Card Account when Order Item is" from Invoiced to Ordered, to be able to receive gift card code and use it even if order isn't invoiced yet

#### Marketing - Gift Card Accounts
- Here can see all gift cards

## Enable Store Credits
#### Stores - Configuration - Customers - Customer Configuration - Store Credit Options
Verify that settings are like this -
- Enable Store Credit Functionality - Yes
- Show Store Credit History to Customers - Yes
- Refund Store Credit Automatically - No

Most important part is first one, it should be set to Yes for store credit functionality to work
