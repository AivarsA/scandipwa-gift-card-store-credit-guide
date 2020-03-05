# ScandiPWA - Gift Card and Store Credit setup guide

#### 1. Verify that Magento Enterprise edition is installed instead of Community Edition

#### 2. Pull locally these pull requests (to be able to add to cart/wishlist gift card products) - 
https://github.com/scandipwa/quote-graphql/pull/25

https://github.com/scandipwa/wishlist-graphql/pull/7

#### 3. Clone locally these 2 (contains functionality to add/remove gift cards and/or store credits from cart) -
https://github.com/AivarsA/customer-balance-graphql

https://github.com/AivarsA/gift-card-graphql

#### 4. Run setup:upgrade. Re-create containers with "--force-recreate" if necessary
