FORMAT: 1A

# Group Stores

## Get/Update Store [/stores/{storeId}]

+ Parameters
    + storeId (number, required, `12345`) ... A unique ID generated by ShipStation and assigned to each store.

+ Model (application/json)

    + Headers
    
            Authorization: < Enter your Basic Authorization string here >
    
    + Body

            {
                "storeId": 12345,
                "storeName": "WooCommerce Store",
                "marketplaceId": 36,
                "marketplaceName": "WooCommerce",
                "accountName": null,
                "email": null,
                "integrationUrl": "http://shipstation-test.wpengine.com",
                "active": true,
                "companyName": "",
                "phone": "",
                "publicEmail": "",
                "website": "",
                "refreshDate": "2014-12-16T17:47:05.457",
                "lastRefreshAttempt": "2014-12-16T09:47:05.457",
                "createDate": "2014-11-06T15:21:13.223",
                "modifyDate": "2014-11-10T08:02:19.117",
                "autoRefresh": true,
                "statusMappings": [
                    {
                        "orderStatus": "awaiting_payment",
                        "statusKey": "Pending"
                    },
                    {
                        "orderStatus": "awaiting_shipment",
                        "statusKey": "Processing"
                    },
                    {
                        "orderStatus": "shipped",
                        "statusKey": "Completed"
                    },
                    {
                        "orderStatus": "cancelled",
                        "statusKey": "Cancelled"
                    },
                    {
                        "orderStatus": "on_hold",
                        "statusKey": "On-hold"
                    }
                ]
            }

### Get Store [GET]

+ Response 200

    [Get/Update Store][]

### Update Store [PUT]
Updates an existing store. This call does not currently support partial updates. The entire resource must be provided in the body of the request. 

+ Request
    
    [Get/Update Store][]

+ Response 200

    [Get/Update Store][]
