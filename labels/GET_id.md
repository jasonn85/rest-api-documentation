# Contact Label

    GET services/:service_id/contact-labels/:label_id
    
Returns a single [Label].

### User Authorization Classes 
* account

## Parameters
None

## Example
### Request

    GET https://api.zingle.me/v1/services/aff8bc93-6e28-4e70-8770-defa35cdfc1b/contact-labels/13dfba6d-66d2-42e9-9290-2ea9dcf7f91d

### Response
``` json
{
    "status": {
        "text": "OK",
        "status_code": 200,
        "description": null
    },
    "result": {
      "id": "13dfba6d-66d2-42e9-9290-2ea9dcf7f91d",
      "display_name": "VIP",
      "background_color": "#93623a",
      "text_color": "#ffffff",
      "is_global": false,
      "is_automatic": false
    }
}
```

[Label]: README.md
