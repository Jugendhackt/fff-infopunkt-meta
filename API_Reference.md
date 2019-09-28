---
permalink: "/api/"
---
# API Reference
**Base URL:** `https://api.fffinfo.de/`
## Get all strikes
**Warning!** Using this endpoint is not recommended because the query takes a long time and returns a very large dataset.
### Path
```
/strikes/all
```

### Request parameters
None.

### Response example
```json
{
   "code":"SUCCESS",
   "message":"",
   "items":[
      {
         "datetime":"Datum und Uhrzeit",
         "meetingPoint":"Startpunkt / Treffpunkt",
         "searchTitle":"titel",
         "routeLength":"Routenlänge",
         "longitude":0,
         "source":"Telegram chat group, collected bei FFF_Info Bot",
         "description":"Beschreibung",
         "url":"Website Veranstalter (wenn nicht bekannt NONE schreiben)",
         "latitude":0,
         "strikeId":3,
         "endPoint":"Endpunkt",
         "title":"Titel"
      }
   ]
}
```

## Get strike details
### Path
```
/strikes/get
```

### Request parameters
`id` - `GET` - ID of the strike

### Response example
```json
{
   "datetime":"28.09.2019 um 18 Uhr",
   "meetingPoint":"Jugendhaus Riedberg ",
   "searchTitle":"abendessen",
   "routeLength":"5m",
   "longitude":0,
   "source":"Telegram chat group, collected bei FFF_Info Bot",
   "description":"es gibt wieder sehr leckeres Essen im Präsentationsraum",
   "url":"Team FFF Infopunkt",
   "latitude":0,
   "strikeId":2,
   "endPoint":"NONE",
   "title":"Abendessen",
   "code":"SUCCESS",
   "message":""
}
```

## Search by title
### Path
```
/strikes/search/title
```

### Request parameters
`q` - `GET` - Search query

### Response
