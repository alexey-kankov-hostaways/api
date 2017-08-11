## Create a listing

### Request

```shell
curl -X POST \
  http://api.hostaway.com/v1/listings \
  -H 'authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIn0.eyJhdWQiOiIxMDQ1MCIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIiwiaWF0IjoxNDk5NzczMjk4LCJuYmYiOjE0OTk3NzMyOTgsImV4cCI6MTUxNTY3MDg5OCwic3ViIjoiIiwic2NvcGVzIjpbImdlbmVyYWwiXX0.RYS6Gi7iLyhHRAzNRPPMUd5jYlGJ5Psq2ejFLDM5wmD1alAB6CdkTIuyrDrtJzkcAyPBpjKBAtDzGzsVrEUxMU90FJG8UO-AXrhxMN0GVtcWqpT5ndCSx0aWEv2TMAOwLX0uU5BSCSzM0jmS2c21gNzRqW2-kMgLfMwMzkVZhas' \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -d '{
    "propertyTypeId": 1,
    "name": "Beautiful and cozy apartment close to city center",
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
    "homeawayPropertyDescription": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
    "homeawayReservationPaymentDueDays": "111",
    "bookingcomPropertyName": "Beautiful and cozy apartment close to city center",
    "bookingcomPropertyDescription": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
    "listingAmenities": [
        {
            "amenityId": 2
        },
        {
            "amenityId": 3
        }
    ],
    "listingBedTypes": [
        {
            "bedTypeId": 2,
            "quantity": 1
        },
        {
            "bedTypeId": 33,
            "quantity": 1
        }
    ],
    "listingImages": [
        {
            "caption": "Kitche",
            "url": "https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-fmR2QBJ-5jFbWDbHx-WcibQ5gXoSEq9V--FkCGtJ4jRE-591ab75c9816f",
            "sortOrder": 2
        },
        {
            "caption": "hall",
            "url": "https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-QYseNxAOkr9LYYAwx4Vy-CQgo2gA0--lYu2Qqn8fpd3M-591ab82749ca1",
            "sortOrder": 3
        }
    ]
}'
```

```php
<?php

$curl = curl_init();

curl_setopt_array($curl, array(
  CURLOPT_URL => "http://api.hostaway.com/v1/listings",
  CURLOPT_RETURNTRANSFER => true,
  CURLOPT_ENCODING => "",
  CURLOPT_MAXREDIRS => 10,
  CURLOPT_TIMEOUT => 30,
  CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
  CURLOPT_CUSTOMREQUEST => "POST",
  CURLOPT_POSTFIELDS => "{\n    \"propertyTypeId\": 1,\n    \"name\": \"Beautiful and cozy apartment close to city center\",\n    \"description\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"thumbnailUrl\": \"https://a1.muscache.com/im/pictures/78885433/a151f1a8_original.jpg?aki_policy=small\",\n    \"houseRules\": \"Additional rules\",\n    \"keyPickup\": \"Key pickup\",\n    \"specialInstruction\": \"Any special instruction\",\n    \"doorSecurityCode\": \"ddff8\",\n    \"country\": \"Germany\",\n    \"countryCode\": \"DE\",\n    \"state\": \"Bremen\",\n    \"city\": \"Bremerhaven\",\n    \"street\": \"Schulstraße 7\",\n    \"address\": \"Schulstraße 7, Bremerhaven, Bremen 27570, Germany\",\n    \"publicAddress\": \"Bremerhaven, Bremen 27570, Germany\",\n    \"zipcode\": \"27570\",\n    \"price\": 211.62,\n    \"starRating\": 5,\n    \"weeklyDiscount\": 0.71,\n    \"monthlyDiscount\": 0.82,\n    \"propertyRentTax\": 12,\n    \"guestPerPersonPerNightTax\": 10,\n    \"guestStayTax\": 12,\n    \"guestNightlyTax\": 13,\n    \"personCapacity\": 6,\n    \"maxChildrenAllowed\": null,\n    \"maxInfantsAllowed\": null,\n    \"maxPetsAllowed\": null,\n    \"lat\": 53.5403,\n    \"lng\": 8.58936,\n    \"checkInTimeStart\": 12,\n    \"checkInTimeEnd\": 21,\n    \"checkOutTime\": 11,\n    \"cancellationPolicy\": \"strict\",\n    \"squareMeters\": 10,\n    \"roomType\": \"entire_home\",\n    \"bathroomType\": \"shared\",\n    \"bedroomsNumber\": 1,\n    \"bedsNumber\": 1,\n    \"bedType\": \"real_bed\",\n    \"bathroomsNumber\": 1,\n    \"minNights\": 1,\n    \"maxNights\": 1125,\n    \"guestsIncluded\": 3,\n    \"cleaningFee\": 40.32,\n    \"priceForExtraPerson\": 54.01,\n    \"instantBookable\": 0,\n    \"instantBookableLeadTime\": 1,\n    \"allowSameDayBooking\": 2,\n    \"sameDayBookingLeadTime\": 12,\n    \"contactName\": \"contactName\",\n    \"contactSurName\": \"contactSurName\",\n    \"contactPhone1\": \"contactPhone1\",\n    \"contactPhone2\": \"contactPhone2\",\n    \"contactLanguage\": \"contactLanguage\",\n    \"contactEmail\": \"contactEmail@mail.com\",\n    \"contactAddress\": \"contactAddress\",\n    \"language\": \"en\",\n    \"currencyCode\": \"USD\",\n    \"timeZoneName\": \"Europe/Berlin\",\n    \"wifiUsername\": \"un\",\n    \"wifiPassword\": \"pass\",\n    \"cleannessStatus\": null,\n    \"cleaningInstruction\": null,\n    \"cleannessStatusUpdatedOn\": null,\n    \"homeawayPropertyName\": \"Beautiful and cozy apartment close to city center\",\n    \"homeawayPropertyDescription\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"homeawayReservationPaymentDueDays\": \"111\",\n    \"bookingcomPropertyName\": \"Beautiful and cozy apartment close to city center\",\n    \"bookingcomPropertyDescription\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"listingAmenities\": [\n        {\n            \"amenityId\": 2\n        },\n        {\n            \"amenityId\": 3\n        }\n    ],\n    \"listingBedTypes\": [\n        {\n            \"bedTypeId\": 2,\n            \"quantity\": 1\n        },\n        {\n            \"bedTypeId\": 33,\n            \"quantity\": 1\n        }\n    ],\n    \"listingImages\": [\n        {\n            \"caption\": \"Kitche\",\n            \"url\": \"https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-fmR2QBJ-5jFbWDbHx-WcibQ5gXoSEq9V--FkCGtJ4jRE-591ab75c9816f\",\n            \"sortOrder\": 2\n        },\n        {\n            \"caption\": \"hall\",\n            \"url\": \"https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-QYseNxAOkr9LYYAwx4Vy-CQgo2gA0--lYu2Qqn8fpd3M-591ab82749ca1\",\n            \"sortOrder\": 3\n        }\n    ]\n}",
  CURLOPT_HTTPHEADER => array(
    "authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIn0.eyJhdWQiOiIxMDQ1MCIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIiwiaWF0IjoxNDk5NzczMjk4LCJuYmYiOjE0OTk3NzMyOTgsImV4cCI6MTUxNTY3MDg5OCwic3ViIjoiIiwic2NvcGVzIjpbImdlbmVyYWwiXX0.RYS6Gi7iLyhHRAzNRPPMUd5jYlGJ5Psq2ejFLDM5wmD1alAB6CdkTIuyrDrtJzkcAyPBpjKBAtDzGzsVrEUxMU90FJG8UO-AXrhxMN0GVtcWqpT5ndCSx0aWEv2TMAOwLX0uU5BSCSzM0jmS2c21gNzRqW2-kMgLfMwMzkVZhas",
    "cache-control: no-cache",
    "content-type: application/json",
  ),
));

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
  echo "cURL Error #:" . $err;
} else {
  echo $response;
}
```

```javascript
var data = JSON.stringify({
  "propertyTypeId": 1,
  "name": "Beautiful and cozy apartment close to city center",
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
  "homeawayPropertyDescription": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
  "homeawayReservationPaymentDueDays": "111",
  "bookingcomPropertyName": "Beautiful and cozy apartment close to city center",
  "bookingcomPropertyDescription": "In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.",
  "listingAmenities": [
    {
      "amenityId": 2
    },
    {
      "amenityId": 3
    }
  ],
  "listingBedTypes": [
    {
      "bedTypeId": 2,
      "quantity": 1
    },
    {
      "bedTypeId": 33,
      "quantity": 1
    }
  ],
  "listingImages": [
    {
      "caption": "Kitche",
      "url": "https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-fmR2QBJ-5jFbWDbHx-WcibQ5gXoSEq9V--FkCGtJ4jRE-591ab75c9816f",
      "sortOrder": 2
    },
    {
      "caption": "hall",
      "url": "https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-QYseNxAOkr9LYYAwx4Vy-CQgo2gA0--lYu2Qqn8fpd3M-591ab82749ca1",
      "sortOrder": 3
    }
  ]
});

var xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === 4) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "http://api.hostaway.com/v1/listings");
xhr.setRequestHeader("authorization", "Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIn0.eyJhdWQiOiIxMDQ1MCIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIiwiaWF0IjoxNDk5NzczMjk4LCJuYmYiOjE0OTk3NzMyOTgsImV4cCI6MTUxNTY3MDg5OCwic3ViIjoiIiwic2NvcGVzIjpbImdlbmVyYWwiXX0.RYS6Gi7iLyhHRAzNRPPMUd5jYlGJ5Psq2ejFLDM5wmD1alAB6CdkTIuyrDrtJzkcAyPBpjKBAtDzGzsVrEUxMU90FJG8UO-AXrhxMN0GVtcWqpT5ndCSx0aWEv2TMAOwLX0uU5BSCSzM0jmS2c21gNzRqW2-kMgLfMwMzkVZhas");
xhr.setRequestHeader("content-type", "application/json");
xhr.setRequestHeader("cache-control", "no-cache");

xhr.send(data);
```

```java
OkHttpClient client = new OkHttpClient();

MediaType mediaType = MediaType.parse("application/json");
RequestBody body = RequestBody.create(mediaType, "{\n    \"propertyTypeId\": 1,\n    \"name\": \"Beautiful and cozy apartment close to city center\",\n    \"description\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"thumbnailUrl\": \"https://a1.muscache.com/im/pictures/78885433/a151f1a8_original.jpg?aki_policy=small\",\n    \"houseRules\": \"Additional rules\",\n    \"keyPickup\": \"Key pickup\",\n    \"specialInstruction\": \"Any special instruction\",\n    \"doorSecurityCode\": \"ddff8\",\n    \"country\": \"Germany\",\n    \"countryCode\": \"DE\",\n    \"state\": \"Bremen\",\n    \"city\": \"Bremerhaven\",\n    \"street\": \"Schulstraße 7\",\n    \"address\": \"Schulstraße 7, Bremerhaven, Bremen 27570, Germany\",\n    \"publicAddress\": \"Bremerhaven, Bremen 27570, Germany\",\n    \"zipcode\": \"27570\",\n    \"price\": 211.62,\n    \"starRating\": 5,\n    \"weeklyDiscount\": 0.71,\n    \"monthlyDiscount\": 0.82,\n    \"propertyRentTax\": 12,\n    \"guestPerPersonPerNightTax\": 10,\n    \"guestStayTax\": 12,\n    \"guestNightlyTax\": 13,\n    \"personCapacity\": 6,\n    \"maxChildrenAllowed\": null,\n    \"maxInfantsAllowed\": null,\n    \"maxPetsAllowed\": null,\n    \"lat\": 53.5403,\n    \"lng\": 8.58936,\n    \"checkInTimeStart\": 12,\n    \"checkInTimeEnd\": 21,\n    \"checkOutTime\": 11,\n    \"cancellationPolicy\": \"strict\",\n    \"squareMeters\": 10,\n    \"roomType\": \"entire_home\",\n    \"bathroomType\": \"shared\",\n    \"bedroomsNumber\": 1,\n    \"bedsNumber\": 1,\n    \"bedType\": \"real_bed\",\n    \"bathroomsNumber\": 1,\n    \"minNights\": 1,\n    \"maxNights\": 1125,\n    \"guestsIncluded\": 3,\n    \"cleaningFee\": 40.32,\n    \"priceForExtraPerson\": 54.01,\n    \"instantBookable\": 0,\n    \"instantBookableLeadTime\": 1,\n    \"allowSameDayBooking\": 2,\n    \"sameDayBookingLeadTime\": 12,\n    \"contactName\": \"contactName\",\n    \"contactSurName\": \"contactSurName\",\n    \"contactPhone1\": \"contactPhone1\",\n    \"contactPhone2\": \"contactPhone2\",\n    \"contactLanguage\": \"contactLanguage\",\n    \"contactEmail\": \"contactEmail@mail.com\",\n    \"contactAddress\": \"contactAddress\",\n    \"language\": \"en\",\n    \"currencyCode\": \"USD\",\n    \"timeZoneName\": \"Europe/Berlin\",\n    \"wifiUsername\": \"un\",\n    \"wifiPassword\": \"pass\",\n    \"cleannessStatus\": null,\n    \"cleaningInstruction\": null,\n    \"cleannessStatusUpdatedOn\": null,\n    \"homeawayPropertyName\": \"Beautiful and cozy apartment close to city center\",\n    \"homeawayPropertyDescription\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"homeawayReservationPaymentDueDays\": \"111\",\n    \"bookingcomPropertyName\": \"Beautiful and cozy apartment close to city center\",\n    \"bookingcomPropertyDescription\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"listingAmenities\": [\n        {\n            \"amenityId\": 2\n        },\n        {\n            \"amenityId\": 3\n        }\n    ],\n    \"listingBedTypes\": [\n        {\n            \"bedTypeId\": 2,\n            \"quantity\": 1\n        },\n        {\n            \"bedTypeId\": 33,\n            \"quantity\": 1\n        }\n    ],\n    \"listingImages\": [\n        {\n            \"caption\": \"Kitche\",\n            \"url\": \"https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-fmR2QBJ-5jFbWDbHx-WcibQ5gXoSEq9V--FkCGtJ4jRE-591ab75c9816f\",\n            \"sortOrder\": 2\n        },\n        {\n            \"caption\": \"hall\",\n            \"url\": \"https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-QYseNxAOkr9LYYAwx4Vy-CQgo2gA0--lYu2Qqn8fpd3M-591ab82749ca1\",\n            \"sortOrder\": 3\n        }\n    ]\n}");
Request request = new Request.Builder()
  .url("http://api.hostaway.com/v1/listings")
  .post(body)
  .addHeader("authorization", "Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIn0.eyJhdWQiOiIxMDQ1MCIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIiwiaWF0IjoxNDk5NzczMjk4LCJuYmYiOjE0OTk3NzMyOTgsImV4cCI6MTUxNTY3MDg5OCwic3ViIjoiIiwic2NvcGVzIjpbImdlbmVyYWwiXX0.RYS6Gi7iLyhHRAzNRPPMUd5jYlGJ5Psq2ejFLDM5wmD1alAB6CdkTIuyrDrtJzkcAyPBpjKBAtDzGzsVrEUxMU90FJG8UO-AXrhxMN0GVtcWqpT5ndCSx0aWEv2TMAOwLX0uU5BSCSzM0jmS2c21gNzRqW2-kMgLfMwMzkVZhas")
  .addHeader("content-type", "application/json")
  .addHeader("cache-control", "no-cache")
  .build();

Response response = client.newCall(request).execute();
```

```python
import http.client

conn = http.client.HTTPConnection("api.hostaway.com")

payload = "{\n    \"propertyTypeId\": 1,\n    \"name\": \"Beautiful and cozy apartment close to city center\",\n    \"description\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"thumbnailUrl\": \"https://a1.muscache.com/im/pictures/78885433/a151f1a8_original.jpg?aki_policy=small\",\n    \"houseRules\": \"Additional rules\",\n    \"keyPickup\": \"Key pickup\",\n    \"specialInstruction\": \"Any special instruction\",\n    \"doorSecurityCode\": \"ddff8\",\n    \"country\": \"Germany\",\n    \"countryCode\": \"DE\",\n    \"state\": \"Bremen\",\n    \"city\": \"Bremerhaven\",\n    \"street\": \"Schulstraße 7\",\n    \"address\": \"Schulstraße 7, Bremerhaven, Bremen 27570, Germany\",\n    \"publicAddress\": \"Bremerhaven, Bremen 27570, Germany\",\n    \"zipcode\": \"27570\",\n    \"price\": 211.62,\n    \"starRating\": 5,\n    \"weeklyDiscount\": 0.71,\n    \"monthlyDiscount\": 0.82,\n    \"propertyRentTax\": 12,\n    \"guestPerPersonPerNightTax\": 10,\n    \"guestStayTax\": 12,\n    \"guestNightlyTax\": 13,\n    \"personCapacity\": 6,\n    \"maxChildrenAllowed\": null,\n    \"maxInfantsAllowed\": null,\n    \"maxPetsAllowed\": null,\n    \"lat\": 53.5403,\n    \"lng\": 8.58936,\n    \"checkInTimeStart\": 12,\n    \"checkInTimeEnd\": 21,\n    \"checkOutTime\": 11,\n    \"cancellationPolicy\": \"strict\",\n    \"squareMeters\": 10,\n    \"roomType\": \"entire_home\",\n    \"bathroomType\": \"shared\",\n    \"bedroomsNumber\": 1,\n    \"bedsNumber\": 1,\n    \"bedType\": \"real_bed\",\n    \"bathroomsNumber\": 1,\n    \"minNights\": 1,\n    \"maxNights\": 1125,\n    \"guestsIncluded\": 3,\n    \"cleaningFee\": 40.32,\n    \"priceForExtraPerson\": 54.01,\n    \"instantBookable\": 0,\n    \"instantBookableLeadTime\": 1,\n    \"allowSameDayBooking\": 2,\n    \"sameDayBookingLeadTime\": 12,\n    \"contactName\": \"contactName\",\n    \"contactSurName\": \"contactSurName\",\n    \"contactPhone1\": \"contactPhone1\",\n    \"contactPhone2\": \"contactPhone2\",\n    \"contactLanguage\": \"contactLanguage\",\n    \"contactEmail\": \"contactEmail@mail.com\",\n    \"contactAddress\": \"contactAddress\",\n    \"language\": \"en\",\n    \"currencyCode\": \"USD\",\n    \"timeZoneName\": \"Europe/Berlin\",\n    \"wifiUsername\": \"un\",\n    \"wifiPassword\": \"pass\",\n    \"cleannessStatus\": null,\n    \"cleaningInstruction\": null,\n    \"cleannessStatusUpdatedOn\": null,\n    \"homeawayPropertyName\": \"Beautiful and cozy apartment close to city center\",\n    \"homeawayPropertyDescription\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"homeawayReservationPaymentDueDays\": \"111\",\n    \"bookingcomPropertyName\": \"Beautiful and cozy apartment close to city center\",\n    \"bookingcomPropertyDescription\": \"In a classic Bremerhaven house we rent out our apartment which has a living room, bed room and is close to all the restaurants and nightlife.\",\n    \"listingAmenities\": [\n        {\n            \"amenityId\": 2\n        },\n        {\n            \"amenityId\": 3\n        }\n    ],\n    \"listingBedTypes\": [\n        {\n            \"bedTypeId\": 2,\n            \"quantity\": 1\n        },\n        {\n            \"bedTypeId\": 33,\n            \"quantity\": 1\n        }\n    ],\n    \"listingImages\": [\n        {\n            \"caption\": \"Kitche\",\n            \"url\": \"https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-fmR2QBJ-5jFbWDbHx-WcibQ5gXoSEq9V--FkCGtJ4jRE-591ab75c9816f\",\n            \"sortOrder\": 2\n        },\n        {\n            \"caption\": \"hall\",\n            \"url\": \"https://s3-us-west-2.amazonaws.com/hostaway-platform-dev/listing/10450-40160-QYseNxAOkr9LYYAwx4Vy-CQgo2gA0--lYu2Qqn8fpd3M-591ab82749ca1\",\n            \"sortOrder\": 3\n        }\n    ]\n}"

headers = {
    'authorization': "Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIn0.eyJhdWQiOiIxMDQ1MCIsImp0aSI6IjJjZGRkYzNiZWU3OGEyZTA5NDgzNmZiYzE3MTQ3M2EwNjlkYTZlYzRjNmRlZDc1NTAzMWYzMzNmODVjYmQyMzI0Y2E4MTk0NzNkYzkxNjYzIiwiaWF0IjoxNDk5NzczMjk4LCJuYmYiOjE0OTk3NzMyOTgsImV4cCI6MTUxNTY3MDg5OCwic3ViIjoiIiwic2NvcGVzIjpbImdlbmVyYWwiXX0.RYS6Gi7iLyhHRAzNRPPMUd5jYlGJ5Psq2ejFLDM5wmD1alAB6CdkTIuyrDrtJzkcAyPBpjKBAtDzGzsVrEUxMU90FJG8UO-AXrhxMN0GVtcWqpT5ndCSx0aWEv2TMAOwLX0uU5BSCSzM0jmS2c21gNzRqW2-kMgLfMwMzkVZhas",
    'content-type': "application/json",
    'cache-control': "no-cache"
    }

conn.request("POST", "/v1/listings", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

`POST https://api.hostaway.com/v1/listings`

A listing object should be provided in the request body.

### Response

The created listing object or error response.