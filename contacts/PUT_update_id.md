# Update Contact

    PUT services/:service_id/contacts/:contact_id
    
Updates a new Contact for the specified Service and returns the updated [Contact Object]

## Parameters
None

## Example
### Request

    PUT https://api.zingle.me/v1/services/aff7bc93-6e28-4e70-8770-defa35cdfc1b/contacts/f119fe3b-67e2-4b59-b605-5586616978d0


#### Request Body    
```json
{
  "is_starred": true,
  "custom_field_values": [
    {
      "custom_field_id": "56c70519-6c70-40e5-904e-7652e54a07b6",
      "value": "Rebeka"
    }
  ]
}
```

### Response
``` json
{
  "status": {
    "text": "OK",
    "status_code": 200,
    "description": null
  },
  "result": {
    "id": "f119fe3b-67e2-4b59-b605-5586616978d0",
    "is_confirmed": true,
    "is_starred": true,
    "created_at": 1442877113,
    "updated_at": 1442877113,
    "last_message": {
      "id": null,
      "body": null,
      "created_at": null
    },
    "channels": [],
    "custom_field_values": [
      {
        "value": "Rebeka",
        "selected_custom_field_option_id": null,
        "custom_field": {
          "id": "56c70519-6c70-40e5-904e-7652e54a07b6",
          "display_name": "First Name",
          "is_global": true,
          "options": []
        }
      }
    ],
    "labels": []
  }
}
```

[Contact Object]: README.md