# Product Removed from Wishlist

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "remove_from_wishlist",
  "detailed_event": "Product Removed from Wishlist",
    "ecommerce": {
        "currency": "<currency>",
        "identifier": "<identifier>",
        "items": [
            {
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
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.identifier|string|Captures a unique identifier for each wishlist|12345, 435678, 34567, XCV456, XCV876|||||||
|ecommerce.items[n].item_brand|string|Item brand|Gucci|||||||
|ecommerce.items[n].item_color|string|Count of time that cart popups were displayed to visitors.|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].item_price_tier|string|Captures the price type \(i.e. List, Markdown, Clearance, Bundle\) associated with a product.|Good, Better, Best, Bronze, Silver, Gold|||||||
|ecommerce.items[n].item_price_type|string|Captures the page name within which CTA links are used.|1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|ecommerce.items[n].item_product_line|string|Captures the product SKU \(stock keeping unit\) associated with products.|Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|ecommerce.items[n].item_trademarked_technology|string|Count of times that visitors click on a Call to Action \(CTA\) link.|Stainmaster, GoreTex, WeatherShield|||||||
|ecommerce.items[n].sku|string|Captures the ID associated with CTA links used.|34567890, 4567890, 00155-large-cornflower|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




