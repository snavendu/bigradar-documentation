# Create a contact

>Our Contacts API is a central place to gather all information and take actions on your contacts, such as fetching, searching, creating, updating, and deleting.


### Example Request and Response  of creating an user

<!-- tabs:start -->

#### **Request**
```
$ curl https://app.bigradar.io/api/users \
-X POST \
-H 'Authorization:Bearer <Your access token>' \
-H 'Accept:application/json'
-H 'Content-Type: application/json' -d


{
	"email": "wash@serenity.io",
	"phone": "+1123456789",
	"name": "Hoban Washburn",
    "data": {
      "paid_subscriber": true,
      "monthly_spend": 155.5,
      "team_mates": 1
    }
}
```

#### **Response**

### If Contacts synced successfully
```
HTTP/1.1 200 OK
  { 
    "type": "user",
    "status": 1,
    "isTmp": false,
    "_id": "60c8678eff91025979501bb8",
    "name": "Hoban Washburn",
    "email": "wash@serenity.io",
    "phone": "+1123456789",
    "organization": "1034ad5",
    "parentId": "60c83da3cffc54344b1605ab",
    "ref": "WkLrs7IZE",
    "organizations": [],
    "sync": [],
    "data": {
      "paid_subscriber": true,
      "monthly_spend": 155.5,
      "team_mates": 1
	  },
    "created_at": 2021-03-15T08:23:13.917+00:00,
	  "updated_at": 2021-03-15T08:23:13.917+00:00,
    "__v": 0
  }
```

### If Contact already exists
```
HTTP/1.1 422 Unprocessable Entity

{
  "message": "Email address already exists"
}

```
<!-- tabs:end -->
| attribute | type | discription |
| --------- | ----------- | ------ |
|email|string|email of the contact|
|name|string|name of the contact|
|phone|string|phone of the contact|
|data|Object|its a custom or extra data you want to provide with contact |


