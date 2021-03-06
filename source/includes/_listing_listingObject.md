## Listing object

```json
{
    "id": 40160,
    "propertyTypeId": 1,
    "name": "Beautiful and cozy apartment close to city center",
    "externalListingName": "Beautiful and cozy apartment close to city center",
    "internalListingName": "Property #3",
    "description": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
    "thumbnailUrl": "https://a1.muscache.com/im/pictures/78885433/a151f1a8_original.jpg?aki_policy=small",
    "houseRules": "Additional rules",
    "keyPickup": "Key pickup",
    "specialInstruction": "Any special instruction",
    "doorSecurityCode": "ddff8",
    "country": "Germany",
    "countryCode": "DE",
    "state": "Bremen",
    "city": "Bremerhaven",
    "street": "Schulstraße 7",
    "address": "Schulstraße 7, Bremerhaven, Bremen 27570, Germany",
    "publicAddress": "Bremerhaven, Bremen 27570, Germany",
    "zipcode": "27570",
    "price": 211.62,
    "starRating": 5,
    "weeklyDiscount": 0.71,
    "monthlyDiscount": 0.82,
    "propertyRentTax": 12,
    "guestPerPersonPerNightTax": 10,
    "guestStayTax": 12,
    "guestNightlyTax": 13,
    "refundableDamageDeposit": 15,
    "personCapacity": 6,
    "maxChildrenAllowed": null,
    "maxInfantsAllowed": null,
    "maxPetsAllowed": null,
    "lat": 53.5403,
    "lng": 8.58936,
    "checkInTimeStart": 12,
    "checkInTimeEnd": 21,
    "checkOutTime": 11,
    "cancellationPolicy": "strict",
    "squareMeters": 10,
    "roomType": "entire_home",
    "bathroomType": "shared",
    "bedroomsNumber": 1,
    "bedsNumber": 1,
    "bedType": "real_bed",
    "bathroomsNumber": 1,
    "minNights": 1,
    "maxNights": 1125,
    "guestsIncluded": 3,
    "cleaningFee": 40.32,
    "priceForExtraPerson": 54.01,
    "instantBookable": 0,
    "instantBookableLeadTime": 1,
    "allowSameDayBooking": 2,
    "sameDayBookingLeadTime": 12,
    "contactName": "contactName",
    "contactSurName": "contactSurName",
    "contactPhone1": "contactPhone1",
    "contactPhone2": "contactPhone2",
    "contactLanguage": "contactLanguage",
    "contactEmail": "contactEmail@mail.com",
    "contactAddress": "contactAddress",
    "language": "en",
    "currencyCode": "USD",
    "timeZoneName": "Europe/Berlin",
    "wifiUsername": "un",
    "wifiPassword": "pass",
    "cleannessStatus": null,
    "cleaningInstruction": null,
    "cleannessStatusUpdatedOn": null,
    "homeawayPropertyName": "Beautiful and cozy apartment close to city center",
    "homeawayPropertyHeadline": "Beautiful and cozy apartment close to city center with a living room and bed room",
    "homeawayPropertyDescription": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
    "bookingcomPropertyName": "Beautiful and cozy apartment close to city center",
    "bookingcomPropertyDescription": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
    "invoicingContactName": "Name",
    "invoicingContactSurName": "Surname",
    "invoicingContactPhone1": "+11122334456",
    "invoicingContactPhone2": "+11122334456",
    "invoicingContactLanguage": "en",
    "invoicingContactEmail": "invoice@company.com",
    "invoicingContactAddress": "221B Baker Street",
    "invoicingContactCity": "London",
    "invoicingContactZipcode": "110011",
    "invoicingContactCountry": "UK",
    "propertyLicenseNumber": null,
    "propertyLicenseType": null,
    "propertyLicenseIssueDate": null,
    "propertyLicenseExpirationDate": null,  
    "listingAmenities": [
        {
            "id": 3449,
            "amenityId": 2
        },
        {
            "id": 3444,
            "amenityId": 3
        }
    ],
    "listingBedTypes": [
        {
            "id": 1,
            "bedTypeId": 2,
            "quantity": 1
        },
        {
            "id": 2,
            "bedTypeId": 33,
            "quantity": 1
        }
    ],
    "listingImages": [
        {
            "id": 877,
            "caption": "Kitche",
            "url": "https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-fmR2QBJ-5jFbWDbHx-WcibQ5gXoSEq9V--FkCGtJ4jRE-591ab75c9816f",
            "sortOrder": 1
        },
        {
            "id": 1027,
            "caption": "hall",
            "url": "https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-QYseNxAOkr9LYYAwx4Vy-CQgo2gA0--lYu2Qqn8fpd3M-591ab82749ca1",
            "sortOrder": 2
        }
    ]
}
```

Some fields which is marked by asterisk (*) are required to change listing status to `complete`.
Only `complete` listing can be activated for synchronization. 

Property | Required | Type | Description
-------- | -------- | ---- | ----------- 
`id` | yes | int | 
`propertyTypeId` | no | int | Identifier of propertyType object.
`name` | yes | string | 
`externalListingName` | yes | string | The same as `name`. 
`internalListingName` | no | string |
`description` | no | string | 
`thumbnailUrl` | no | string | 
`houseRules` | no | string | 
`keyPickup` | no | string | 
`specialInstruction` | no | string | 
`doorSecurityCode` | no | string | 
`country` | no | string | 
`countryCode` | no | string | 
`state` | no | string | 
`city` | no | string | 
`street` | no | string | 
`address` | yes* | string | 
`publicAddress` | no | string | 
`zipcode` | no | string | 
`price` | yes* | float | 
`starRating` | no | int | 
`weeklyDiscount` | no | float | 
`monthlyDiscount` | no | float | 
`propertyRentTax` | no | float | 
`guestPerPersonPerNightTax` | no | float | 
`guestStayTax` | no | float | 
`guestNightlyTax` | no | float |
`refundableDamageDeposit` | no | float |  
`personCapacity` | no | int | 
`maxChildrenAllowed` | no | int | 
`maxInfantsAllowed` | no | int | 
`maxPetsAllowed` | no | int | 
`lat` | no | float | Latitude.
`lng` | no | float | Longitude.
`checkInTimeStart` | no | int | Accepted values are 0-23
`checkInTimeEnd` | no | int | Accepted values are 0-23
`checkOutTime` | no | int | 
`cancellationPolicy` | no | string | One of: flexible, moderate, strict.
`squareMeters` | no | int | 
`roomType` | no | string | One of: entire_home, private_room, shared_room.
`bathroomType` | no | string | One of: private, shared.
`bedroomsNumber` | no | int | 
`bedsNumber` | no | int | 
`bathroomsNumber` | no | int | 
`minNights` | no | int | 
`maxNights` | no | int | 
`guestsIncluded` | yes* | int | 
`cleaningFee` | no | float | 
`priceForExtraPerson` | yes* | float | 
`instantBookable` | no | bool | 
`instantBookableLeadTime` | no | int | 
`allowSameDayBooking` | no | int | 
`sameDayBookingLeadTime` | no | int | 
`contactName` | no | string | 
`contactSurName` | no | string | 
`contactPhone1` | no | string | 
`contactPhone2` | no | string | 
`contactLanguage` | no | string | 
`contactEmail` | no | string | 
`contactAddress` | no | string | 
`language` | no | string | 
`currencyCode` | yes* | string | 
`timeZoneName` | no | string | 
`wifiUsername` | no | string | 
`wifiPassword` | no | string | 
`cleannessStatus` | no | string | 
`cleaningInstruction` | no | string | 
`cleannessStatusUpdatedOn` | no | datetime | 
`homeawayPropertyName` | no | string | 
`homeawayPropertyHeadline` | no | string | 
`homeawayPropertyDescription` | no | string | 
`bookingcomPropertyName` | no | string | 
`bookingcomPropertyDescription` | no | string | 
`invoicingContactName` | no | string | 
`invoicingContactSurName` | no | string | 
`invoicingContactPhone1` | no | string | 
`invoicingContactPhone2` | no | string | 
`invoicingContactEmail` | no | string | 
`invoicingContactAddress` | no | string | 
`invoicingContactCity` | no | string | 
`invoicingContactZipcode` | no | string | 
`invoicingContactCountry` | no | string | 
`propertyLicenseNumber`  | no | string |
`propertyLicenseType` | no | string |
`propertyLicenseIssueDate` | no | date (YYYY-MM-DD) |
`propertyLicenseExpirationDate` | no | date (YYYY-MM-DD) |
`listingAmenities` | no | array | Array of listingAmenity objects.
`listingBedTypes` | no | array | Array of listingBedType objects.
`listingImages` | no | array | Array of listingImage objects.
