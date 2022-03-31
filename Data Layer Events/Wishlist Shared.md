# Wishlist Shared

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "share_wishlist",
  "detailed_event": "Wishlist Shared",
    "ecommerce": {
        "currency": "<currency>",
        "identifier": "<identifier>",
        "items": [
            {
                "item_price_type": "<item_price_type>",
                "price": "<price>",
                "sku": "<sku>"
            }
        ],
        "value": "<value>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|Specifies the currency to be used for an Adobe Analytics currency events.  Enables exchange rate calucations at the time of data caputure.|USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|ecommerce.identifier|string|Captures a unique identifier for each wishlist|12345, 435678, 34567, XCV456, XCV876|||||||
|ecommerce.items[n].item_price_type|string|Captures the page name within which CTA links are used.|1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|ecommerce.items[n].price|string|Amount of money associated with products shared from a wishlist.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|ecommerce.items[n].sku|string|Captures the ID associated with CTA links used.|34567890, 4567890, 00155-large-cornflower|||||||
|ecommerce.value|string|Captures the total monetary value of each wishlist.|5, 20, 10.22|^[0-9]*(\.[0-9]{1,2})?$||||||




