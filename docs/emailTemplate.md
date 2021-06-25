# Integerate BigRadar email template  to send email

>Our email template allows to send the email to the designated email,and it is quite simple to integerate.
### Example Request and Response  of retreiving a contact

<!-- tabs:start -->

#### **Request**
```
$ curl https://b.bigradar.co.uk/api/templates/:template-name/send \
-X POST \
-H 'Authorization:<Your bigradar access token>' \
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

```
HTTP/1.1 200 OK
{
    "status": "ok",
    "message": "Email has been sent to navendu6895@gmail.com"
}
```


<!-- tabs:end -->
