## NOTE
Point of Sale System (POSS) is a piece of software I worked on sometimes in the past but the repository has been private since and not ready to make it public so I'm only just lifting the README there here public to make publicly what the software does. if interested in the software, you can reach out [via email](mailto:adedayomatt@gmail.com) or [via WhatsApp](https://wa.me/2348139004572).


## Point of Sale System
This application is for managing goods or products and their sales. It can be used in supermarket or stores.

## What it can do

- Manage different kind of goods. When adding new product, you have the option to add it as a simple product or variable product. Variable products refers to poducts that has attribute (e.g color, size). Products can also be converted from simple to variable and vice versa
- Comprehensive insight of stocks. This application will give insight to products collectively and individually, you will be able to see the monetary value of your stocks, how much profit you have made and your prospective profit.
- Graphical representation. You can easily view your sales on a simple column chart (credit to [FusionChart](https://www.fusioncharts.com))
- Transaction Filter. You can view your transactions (including sales and stock updates) at dfferent times or within a range of period
- Different Levels of users. The application allow for two different levels of users - Manager and Attendant - with different priviledges. The manager will be able to add products, create categories, open/close attendants' desks, view products insight. The attendant can add product to cart and checkout.
- Multiple sale. The application uses [Laravel shopping cart](https://github.com/Crinsane/LaravelShoppingcart) to add multiple items to cart for one customer.
- Receipt printing. The application uses [barryvdh/laravel-dompdf](https://github.com/barryvdh/laravel-dompdf) to generate receipt that can be printed when a cart is checked out. The receipt is configured for Thermal printer of paper with width of 58mm.
- Receipt verification. Every cart used for sale by the attendant has unique reference and are saved and also inscribed on the customer's receipt.This can be used for verification of customer's receipt incase of any issue.
## New in V2.0
- System central control. The whole system can now be controlled by a superadmin.
- Added premium package to the app. The package plan is only changeable by  the superadmin.
- Multiple shop. You can now use the application to manage more than one store.(Premium only) 
- New user priviledge Admin. A new user level has been added (admin). The admin will be charge of all the shops while managers are restricted to the shop assigned to them.
- Services. Not only product you can now manage, services can also be added and recorded by attendant. Service receipts can also be verified.
- Aesthaetic control. You can now set the color of shops different, cool isn't it???
- Control Low stocks notification. You can now choose to enable low stock warning and also specify the number of remaining to be considered as low

## New in V2.1
- Barcode. Barcode are now available. You can now attach barcode to product or generate one if product doesn't have. You can now also use barcode scanner to add product to cart. Barcode credit: [milon/barcode](https://github.com/milon/barcode)
- sales can now be revoked.
- Sales receipts are now reprintable as many times as you want. meanwhile the issued date will still be maintained on the receipt

## New in V2.2
- Backup Feature. You can now backup your data - both code base and database in a zip file for future restoration if need arises. Backup credit: [spatie/laravel-backup](https://github.com/spatie/laravel-backup)

## New in v3.0
- Upgraded Php version requirement from 7.1.3 to 7.4
- Upgraded Laravel to 7.3.1
- Upgraded other dependencies and use specific versions
- Upgraded [Laravel shopping cart by Crinsane](https://github.com/Crinsane/LaravelShoppingcart) to [Laravel shopping cart by Bumbummen99 ](https://github.com/bumbummen99/LaravelShoppingcart)
- Following features available only in Premium
    - Receipt printing
    - Receipt verification
    - Control printing receipt or not when checked out from desk
    - Variable product
- Stock batches for price control
- Flexible selling price with price floor 
- Recoding defect for product
- Customer management, customer can be recorded with each sale; either select from existing customers or create new
- Purchase history by each customer
- Customer with highest purchase by item quantity or amount included in sales report
