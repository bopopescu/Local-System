<!-- add-breadcrumbs -->
# Amazon MWS Integration
 The Amazon Connector pulls Products and Sales Orders from Amazon marketplace.
 The synch of Products and Sales Orders is sequential. You have to synch the products before you Synch the Sales Orders.

### How to Setup Amazon MWS Connector?

#### Setting Up Credentials  in ERPNext

You can request the developer credentials from Amazon MWS once you are a registered seller on their website.

 1. Enter the Seller ID, AWS Access Key ID, MWS Auth Token, Secret Key, Market Place ID, Region and Domain.
<img class="screenshot" alt="Setup Credentials" src="{{docs_base_url}}/assets/img/erpnext_integrations/amazon_mws_settings_1.png">

 2. Setup Company, Warehouse, Item Group, Price List, Customer Group, Territory, Customer Type and Account Group.
   The Account Group is used to hold Commission, taxes etc. that Amazon charges.
<img class="screenshot" alt="ERPNext Configurations" src="{{docs_base_url}}/assets/img/erpnext_integrations/amazon_mws_settings_2.png">
 
 3. Setup Synch Configurations.
   Using the After Date, you can synch products and orders created after a particular date. In case you are importing a lot of historic data, it is suggested to start in the reverse chronological order of the After Date and import data in small chunks.
<img class="screenshot" alt="Sync Configurations" src="{{docs_base_url}}/assets/img/erpnext_integrations/amazon_mws_settings_3.png">
After setting up all the configurations, click on Enable Amazon and save the settings. You are now ready to use the
integration.
 
 4. Synch Products
   To synch products, you can click on Synch Products. Once this is successful you should see your Amazon products
   as Items in ERPNext.
<img class="screenshot" alt="Sync Configurations" src="{{docs_base_url}}/assets/img/erpnext_integrations/amazon_mws_settings_4.png">
<img class="screenshot" alt="Sync Configurations" src="{{docs_base_url}}/assets/img/erpnext_integrations/amazon_mws_settings_5.png">
 
 5. Synch Sales Orders
   To synch orders, you can click on Synch Orders. Once this is successful you should see your Amazon Orders
   as Sales Orders in ERPNext. You can also set up scheduler to synch orders automatically.
<img class="screenshot" alt="Sync Configurations" src="{{docs_base_url}}/assets/img/erpnext_integrations/amazon_mws_settings_6.png">

### Note
 
The connector won't handle Order cancellation. If you cancelled any order in Amazon then manually you have to cancel respective Sales Order and other documents in ERPNext.
