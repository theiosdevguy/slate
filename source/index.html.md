---
title: API Reference

language_tabs:
  - json

toc_footers:
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:

search: true
---

# Introduction

CLEANSWEEP API DOCUMENTATION

# Retrieve Listings

> REQUEST:

```json

{
  "email": "sweepdevel@gmail.com",
  "api_key": "1X749576E1",
  "password": "tigerbright99"
}
```

> RESPONSE:

```json

{
  "0": {
    "_id": {
      "$id": "580d2522abb5d4d16d18d43c"
    },
    "FromEMail": "sweepdevel@gmail.com",
    "Privacy": "1",
    "contact_phone_ok": "1",
    "contact_text_ok": "1",
    "contact_phone": null,
    "contact_name": "Test User",
    "PostingTitle": "Timex Watch",
    "Ask": "20",
    "price": "20",
    "GeographicArea": "\nNew Delhi 110092\nDelhi\nIndia",
    "postal_code": "110092",
    "PostingBody": "Timex Watch for sale only 20 dollars",
    "sale_condition": "excellent",
    "see_my_other": "1",
    "sale_manufacturer": "",
    "sale_model": "",
    "sale_size": "",
    "wantamap": "",
    "xstreet0": "",
    "xstreet1": "",
    "city": "",
    "region": null,
    "postal": null,
    "contact_ok": null,
    "created": "2016-10-23 17:01:22",
    "modified": "2016-10-23 17:01:22",
    "posted": "2016-10-23 17:01:22",
    "fingerprint": "CleansweepMobile_52ECC847-6CE1-4EA3-B698-A2140C81F995:987347301007",
    "posting_id": 284,
    "post_status": "DELETE",
    "latitude": 0,
    "longitude": 0,
    "images": [
      "http://km.cleansweep.me/imagecache/284.jpg"
    ],
    "videos": []
  },
  "1": {
    "_id": {
      "$id": "581100a0abb5d4450b9f44c1"
    },
    "FromEMail": "sweepdevel@gmail.com",
    "Privacy": "1",
    "contact_phone_ok": "1",
    "contact_text_ok": "1",
    "contact_phone": null,
    "contact_name": "Test User",
    "PostingTitle": "black android one case",
    "Ask": "200",
    "price": "200",
    "GeographicArea": "\nNew Delhi 110092\nDelhi\nIndia",
    "postal_code": "110092",
    "PostingBody": "Android phone for sale only $200. ",
    "sale_condition": "new",
    "see_my_other": "1",
    "sale_manufacturer": "",
    "sale_model": "",
    "sale_size": "",
    "wantamap": "",
    "xstreet0": "",
    "xstreet1": "",
    "city": "del",
    "city_code": "del",
    "region": null,
    "postal": null,
    "contact_ok": null,
    "created": "2016-10-26 15:14:40",
    "modified": "2016-10-26 15:14:40",
    "posted": "2016-10-26 15:14:40",
    "fingerprint": "CleansweepMobile_373C628A-7DC0-4BBB-9235-21A0946EE4BA:4002429843455",
    "posting_id": 297,
    "post_status": "PENDING",
    "latitude": 28.635813087151,
    "longitude": 77.312304151869,
    "images": [
      "http://km.cleansweep.me/imagecache/297.jpg"
    ],
    "sounds": [
      "http://km.cleansweep.me/audiocache/297.wav"
    ],
    "videos": [
      "http://km.cleansweep.me/videocache/297.mp4"
    ]
  },
  "status": "OK"
}
```

### HTTP Request

`POST http://cleansweep.kimmccann.net/services/postings`




# Register Device

### HTTP Request

`POST http://cleansweep.kimmccann.net/services/register-device`

>REQUEST:

```json
{
  "email": "sweepdevel@gmail.com",
  "deviceid": "CleansweepMobile_412616C6-B887-4BDC-AE29-3B0F4B1F736B",
  "api_key": "1X749576E1",
  "apnid": "a2c8d0fae90c773ae2d868bda68c15943a7b6ff3b5ecf7777c762c5597cd8b38"
}

```
>RESPONSE:

```json
{
  "status": "OK",
  "message": "device registered: CleansweepMobile_412616C6-B887-4BDC-AE29-3B0F4B1F736B",
  "devices": [
    {
      "_id": {
        "$id": "581b372cec82219bd9d2699c"
      },
      "deviceid": "CleansweepMobile_412616C6-B887-4BDC-AE29-3B0F4B1F736B",
      "apnid": "a2c8d0fae90c773ae2d868bda68c15943a7b6ff3b5ecf7777c762c5597cd8b38",
      "email": "sweepdevel@gmail.com",
      "modified": "2016-11-08 08:29:51"
    }
  ]
}
```

This endpoint registers the device on the server with the device's apn id for sending Push Notifications.


# Fetch Cities and City codes

> REQUEST:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```


> RESPONSE:

```json
{
  "cities": [
    {
      "code": "abz",
      "city": "aberdeen",
      "region": "gb",
      "country": "gb"
    },
    {
      "code": "abi",
      "city": "abilene",
      "region": "tx",
      "country": "us"
    },
    {
      "code": "aca",
      "city": "acapulco",
      "region": "mx",
      "country": "mx"
    },
    {
      "code": "adl",
      "city": "adelaide",
      "region": "sa",
      "country": "au"
    },
    {
      "code": "amd",
      "city": "ahmedabad",
      "region": "in",
      "country": "in"
    },
    {
      "code": "cak",
      "city": "akron-canton",
      "region": "oh",
      "country": "us"
    },
    {
      "code": "aby",
      "city": "albany",
      "region": "ga",
      "country": "us"
    },
    {
      "code": "alb",
      "city": "albany",
      "region": "ny",
      "country": "us"
    }
  ],
  "status": "OK"
}
```

This endpoint retrieves all the cities and the city codes required for Craigslist.

### HTTP Request

`POST http://cleansweep.kimmccann.net/services/cities`




# Status update for peerid

> REQUEST:

```json
{
  "peerid": "CleansweepMobile_412616C6-B887-4BDC-AE29-3B0F4B1F736B",
  "status": "ready",
  "latitude": 28.63584879322782,
  "api_key": "1X749576E1",
  "longitude": 77.31228215627122,
  "origin": null
}
```


> RESPONSE:

```json
{
  "status": "OK",
  "message": "",
  "peers": []
}
```

This endpoint updates the status for a peer on server.

### HTTP Request

`POST http://cleansweep.kimmccann.net/services/peerid`
