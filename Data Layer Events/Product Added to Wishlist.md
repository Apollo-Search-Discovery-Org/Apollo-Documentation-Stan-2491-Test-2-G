# Product Added to Wishlist

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "add_to_wishlist",
  "detailed_event": "Product Added to Wishlist",
    "ecommerce": {
        "currency": "<currency>",
        "identifier": "<identifier>",
        "items": [
            {
                "date_added": "<date_added>",
                "item_brand": "<item_brand>",
                "item_color": "<item_color>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "item_price_tier": "<item_price_tier>",
                "item_price_type": "<item_price_type>",
                "item_product_line": "<item_product_line>",
                "item_trademarked_technology": "<item_trademarked_technology>",
                "sku": "<sku>"
            }
        ],
        "multiple_addition_detail": "<multiple_addition_detail>",
        "multiple_additions": <multiple_additions>,
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.identifier|string|Captures a unique identifier for each wishlist|12345, 435678, 34567, XCV456, XCV876|||||||
|ecommerce.items[n].date_added|string|Captures the date when a product was added to a wishlist.|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|ecommerce.items[n].item_brand|string|Item brand|Gucci|||||||
|ecommerce.items[n].item_color|string|Count of time that cart popups were displayed to visitors.|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].item_price_tier|string|Captures the price type \(i.e. List, Markdown, Clearance, Bundle\) associated with a product.|Good, Better, Best, Bronze, Silver, Gold|||||||
|ecommerce.items[n].item_price_type|string|Captures the page name within which CTA links are used.|1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|ecommerce.items[n].item_product_line|string|Captures the product SKU \(stock keeping unit\) associated with products.|Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|ecommerce.items[n].item_trademarked_technology|string|Count of times that visitors click on a Call to Action \(CTA\) link.|Stainmaster, GoreTex, WeatherShield|||||||
|ecommerce.items[n].sku|string|Captures the ID associated with CTA links used.|34567890, 4567890, 00155-large-cornflower|||||||
|ecommerce.multiple_addition_detail|string|Captures how many products of the total displayed were added at the time of an add event \(i.e., cart add, wishlist add, registry add\).|all items, 3 of 5, 2 of 4|||||||
|ecommerce.multiple_additions|boolean|Count of times visitors added multiple items at the time of an event \(i.e., cart add, wishlist add, registry add\).|TRUE, FALSE|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




