# commerce_stock_cap
Drupal 9 module to limit variant stock to stock of a master product

Use case:
I want to sell tickets to a show. I have (2) available variants: (A) 1-ticket for $10 (B) 2-tickets for $18. 
If I want to limit total ticket sales to 100 I can use this custom code to achieve that. 

For variant A, count the stock
For variant B, count the stock (*2)
If total_sold > total_available, then we change the Add-To-Cart button to 'Sold-Out' and disable it

• Product ID of master product must be known and hard-coded
• Variant IDs of that master product must also be known, hard coded, and a logic block to handle each variant ID
