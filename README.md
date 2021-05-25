# official_Kanaree.io_GTM_template
This is the official Kanaree.io Google Tag Manager template. This template is for use with core Kanaree.io data streaming websites. 

# Requirements:
Users of this template will need to have a Kanaree.io account and site key. 

For existing users, you can find your site key inside your console here https://app.mykanaree.com/

For new users, you can register for an account and site key here https://www.kanaree.io/sign-up   

# Template Core Functionality

## Loading the main Kanaree.io tracker (Required): 
  Event Type: Load Main Track
  
  Account ID (Required): This is your unique site id and can be found in your Kanaree.io console.
  
  Page Label (Optional): An optional value used to help organize your data. Usually a meaningful single string descriptor of a page. For product pages it might be a sku for a blog page it might be a title.
  
  Page Type (Optional): An optional categorization of the page to help you organize your data. Usually a meaningful single string grouping of pages. For product pages it might be products and for blog pages it might be blog

  Trigger: Load this script on all pages using the All Pages trigger or the Window Loaded built in triggers. 

  Recommended: In your advanced settings set your “Tag Firing Priority” to a large number to increase the chance of the Kanaree.io tracking script loading early in the queue. 

## Kanaree.io Custom Events (Optional): 

Event Type: Custom Event

Account ID (Required): This is your unique site id and can be found in your Kanaree.io console.
  
Event Category (Required): A required string value used to help organize your data. Usually, a meaningful single string descriptor of a group of events. Example: All ecommerce events might use a category of “Ecommerce”. Data Type: String

Event Action (Optional): An optional string value used to help organize your data. Usually, a meaningful single string descriptor of a user action. Example: An action of a user adding to cart might have an action of “ATC”. Data Type: String 

Event Label (Optional): An optional string value used to help organize your data. Usually, a meaningful single string descriptor of an action. Example: An action of a user adding to cart might have an label of the item added. Data Type: String 

Event Value (Optional): An optional string value used to help organize your data. Usually, a value assigned to a user taking an action. This is not required to be a numeric value and as such can be used in many different ways. Example: An action of a user adding to cart could have the price as value or a customer group. Data Type: String 

## Kanaree.io Set User (Optional): 

Event Type: Set User

Account ID (Required): This is your unique site id and can be found in your Kanaree.io console.
  
User ID (Required): A required string value used to identify and unify customer data. Usually, a meaningful single string descriptor unique to a user. NEVER PASS RAW PERSONALY IDENTIFIABLE INFORMATION. Kanaree.io suggests a Sha256 hash, implementation examples can be found on the Kanaree.io website.  Example: Customer account number. Data Type: String

## Kanaree.io Set User Fields (Optional): 

Event Type: Set User Fields

Account ID (Required): This is your unique site id and can be found in your Kanaree.io console.
  
Key  (Required): A required string value used to identify customer data you are setting. Usually, a meaningful single string descriptor. Example: Customer Group. Data Type: String

Value  (Required): A required string value assigned to a customer that corresponds to the key value. Usually, a meaningful single string descriptor unique to a user. NEVER PASS RAW PERSONALY IDENTIFIABLE INFORMATION. Kanaree.io suggests a Sha256 hash, implementation examples can be found on the Kanaree.io website.  Example: Customer Social ID. Data Type: String



