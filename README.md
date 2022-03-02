# Edgenuity-SIS-Hack
XSS attack on the Edgenuity Student Information System

## API Request Formatting
### SendMessage
```json
{
  "d":
    {
      "MessageIndex": Number,
      "SenderUserIndex": Number,
      "DateTime": String, // "\/Date(ms)\/"
      "Subject": String,
      "Contents": String,
      "Sender": String, // "Lastname, Firstname"
      "SenderPrivilege": String // "STUDENT" || "TEACHER"
      "ArchivedOn": null,
      "Recipients": [{
        "UserIndex": Number,
        "Name": String, // "Lastname, Firstname"
        "ReadOn": null,
        "ArchivedOn": null,
        "RecipientPrivilege": String // "STUDENT" || "TEACHER"
      }],
      "Affiliation": String, // "DISTRICT (IS)"
      "Attachments": Array
     }
}
```
