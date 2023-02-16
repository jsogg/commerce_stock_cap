# commerce_stock_cap<br />
Drupal 9 module to limit variant stock to stock of a master product<br />
<br />
Use case:<br />
I want to sell tickets to a show. I have (2) available variants: (A) 1-ticket for $10 (B) 2-tickets for $18. <br />
If I want to limit total ticket sales to 100 I can use this custom code to achieve that. <br />
<br />
For variant A, count the past sales history qty<br />
For variant B, count the past sales history qty (*2)<br />
If total_sold > total_available, then we change the Add-To-Cart button to 'Sold-Out' and disable it<br />
<br />
• Product ID of master product must be known and hard-coded<br />
• Variant IDs of that master product must also be known, hard coded, and a logic block to handle each variant ID<br />
