# Retrieve a contact

>Our Contacts API is a central place to gather all information and take actions on your contacts, such as fetching, searching, creating, updating, and deleting.

### Example Request and Response  of retreiving a contact

<!-- tabs:start -->

#### **Request**
```
$ curl https://app.bigradar.io/api/users \
-H 'Authorization:Bearer <Your access token>' \
-H 'Accept:application/json'
```

#### **Response**

### If Contacts synced successfully
```
HTTP/1.1 200 OK
{
    "limit": 50,
    "page": 1,
    "pages": 2,
    "total": 60,
    "docs": [
        {
            "emailStatus": {
                "status": "sent"
            },
            "type": "user",
            "status": 0,
            "isTmp": false,
            "_id": "604f1f1f019d973957316744",
            "organization": "1034ad5",
            "ref": "unJPbU-z8",
            "organizations": [],
            "sync": [],
            "tmpName": "Bethel Sipes",
            "browser": {
                "_id": "604f1f1f019d973957316745",
                "name": "Chrome",
                "version": "83.0.4103.116",
                "os": "Linux",
                "os_version": "x86_64",
                "engine": "Blink",
                "cpu": "amd64",
                "device": "",
                "device_model": "",
                "device_vendor": ""
            },
            "createdAt": "2021-03-15T08:47:27.696Z",
            "updatedAt": "2021-06-02T06:10:58.281Z",
            "__v": 0,
            "url": "http://localhost:8001/",
            "email": "snavendu0@gmail.com",
            "name": "D2 Test",
            "lastSeen": "2021-03-15T10:11:50.173Z",
            "data": {
                "label": [
                    "new"
                ]
            },
            "fullname": "D2 Test",
            "id": "604f1f1f019d973957316744"
        },
        {
            "emailStatus": {
                "status": "sent"
            },
            "type": "user",
            "status": 0,
            "isTmp": false,
            "_id": "604f1971019d9739573166c9",
            "organization": "1034ad5",
            "ref": "uuCAw2n9v",
            "organizations": [],
            "sync": [],
            "tmpName": "Nick Littel",
            "browser": {
                "_id": "604f1971019d9739573166ca",
                "name": "Chrome",
                "version": "83.0.4103.116",
                "os": "Linux",
                "os_version": "x86_64",
                "engine": "Blink",
                "cpu": "amd64",
                "device": "",
                "device_model": "",
                "device_vendor": ""
            },
            "createdAt": "2021-03-15T08:23:13.917Z",
            "updatedAt": "2021-05-31T12:05:28.103Z",
            "__v": 0,
            "url": "http://localhost:8001/",
            "email": "fsdf",
            "name": "fsdf",
            "lastSeen": "2021-03-15T08:27:35.116Z",
            "fullname": "fsdf",
            "id": "604f1971019d9739573166c9"
        },
        {
            "emailStatus": {
                "status": "sent"
            },
            "type": "user",
            "status": 1,
            "isTmp": false,
            "_id": "607d64a8f6cace1fcd373cad",
            "data": {
                "label": "Import_Apr_19"
            },
            "name": "bansalgroupshr@gmail.com",
            "email": "bansalgroupshr@gmail.com",
            "createdAt": "2021-04-19T11:08:24.271Z",
            "browser": {
                "_id": "607d64a8f6cace1fcd373cae"
            },
            "location": {
                "_id": "607d64a8f6cace1fcd373caf"
            },
            "organization": "1034ad5",
            "ref": "Gz5sHxmUR0",
            "organizations": [],
            "sync": [],
            "updatedAt": "2021-05-31T12:05:29.217Z",
            "__v": 0,
            "fullname": "bansalgroupshr@gmail.com",
            "id": "607d64a8f6cace1fcd373cad"
        },
        ]
}
```


<!-- tabs:end -->