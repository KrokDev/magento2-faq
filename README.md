# magento2-faq
FAQ Open-Source Module for Magento 2

* As a customer I want to be able look for frequent questions on
  * products
  * FAQ page
    * List all FAQs for the current store, sorted by tags and position
    * Filters by tags (show only tags with available results, an empty tag shouldn't be visible)
    * Filters by product category
  * checkout (cart & checkout)
* As a customer I want to be able to search for a question on the FAQ page
* As a customer if I don't find an answer I want to contact the customer support
* As a customer I want to rate the answer (useful or not)

* As a merchant I want to list all FAQ entries
* As a merchant I want to mass delete FAQ entries of my choice
* As a merchant I want to mass enable/disable FAQ entries of my choice
* As a merchant I want to create a new FAQ entry
  * FAQ entry is represented by:
    * Unique Identifier (text field; composite unique constraint on identifier/store_id)
    * Stores (store field)
    * Customer Group (customer group field; used to show faq for only some of the customers)
    * Question (text field)
    * Short Answer (textarea field)
    * Answer (wysiwyg field)
    * Position (numeric field; used to sort QA in listing)
    * Tags (multiselect field)
    * Products (product links)
    * Rating (numeric field; readonly/disabled)
* As a merchant I want to list all tags
* As a merchant I want to mass delete tags of my choice
* As a merchant I want to create a new tag
  * Tag entry is represented by:
    * Unique Identifier (text field)
    * Title (text field; 1 field by store)
* As a merchant I want to add a Widget to CMS pages, block, widget in order to show a list of FAQs by tags
* As a merchant I want to configure the url key of the FAQ page, by store (it should add/update the url_rewrite entry)
* As a merchant I want to allow roles for specific actions (Create, Read, Update, Delete, Config)
