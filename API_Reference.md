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
