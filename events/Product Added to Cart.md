# Product Added to Cart

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Added to Cart",
    "cart": {
        "additionContext": "<additionContext>",
        "cartID": "<cartID>",
        "cartModifications": "<cartModifications>"
    },
    "eventDetails": {
        "multiAdditionDetail": "<multiAdditionDetail>",
        "multiAdditions": "<multiAdditions>"
    },
    "product": [
        {
            "fulfillment": {
                "method": "<method>"
            },
            "productInfo": {
                "brand": "<brand>",
                "isOutOfStock": "<isOutOfStock>",
                "productID": "<productID>",
                "sku": "<sku>",
                "trademarkedTechnology": "<trademarkedTechnology>"
            },
            "quantity": "<quantity>"
        }
    ]
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|additionContext|string|Conveys the context of a cart addition. |PLP, PDP, Wishlist, Registry|||||||
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|cartID|string|Back-end identifier for a shopping cart|12345, 435678, 34567, XCV456, XCV876|||||||
|cartModifications|integer|Count of times the change in product quantity was the result of a cart modification.||||||||
|isOutOfStock|boolean|Boolean flag indicating that an inventoried product is out of stock. |TRUE, FALSE|||||||
|method|string|Captures the shipping fullfilment method associated with a product.||||||||
|multiAdditionDetail|string|Provides details of multiple product additions to carts, wishlists, registries, etc.|all items, 3 of 5, 2 of 4|||||||
|multiAdditions|boolean|Flag indicating whether multilple products where added to carts, wishlists, registries, etc.|true, false|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|quantity|integer|Integer number of products being acted upon \(added to a cart, removed from wishlist, purchased, reserved\)|1, 2, 3, 4, 5||||1|||
|sku|string|Stock Keeping Unit \(SKU\) Unique Identifier of specific item \(typically\) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|trademarkedTechnology|string|Describes trademarks and\/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||
