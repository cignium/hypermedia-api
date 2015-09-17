# Cignium Hypermedia API

An open source hypermedia type to describe links, schema and validation.

## Example (WIP)

```json
{
  "type": "object",
  "links": [
    {
      "href": "http://people.com/1",
      "rel": "self",
      "title": "John"
    }
  ],
  "errors": [],
  "properties": [
    {
      "errors": [],
      "id": "name",
      "links": [],
      "maxLength": 20,
      "title": "Name",
      "type": "string",
      "value": "John"
    },
    {
      "errors": [],
      "id": "age",
      "links": [],
      "restrictions": {
        "precision": 2,
        "scale": 0
      },
      "title": "Age",
      "type": "number",
      "value": "John"
    },
    {
      "errors": [],
      "id": "address",
      "links": [],
      "properties": [
        {
          "errors": [],
          "id": "street",
          "links": [],
          "title": "Street",
          "type": "string",
          "value": "555 Fifth Avenue"
        },
        {
          "errors": [],
          "id": "city",
          "links": [],
          "title": "City",
          "type": "string",
          "value": "New York"
        }
      ],
      "title": "Address",
      "type": "object"
    },
    {
      "errors": [],
      "items": [
        {
          "errors": [],
          "links": [{
            "href": "http://people.com/update-child-1",
            "rel": "update"
          }],
          "properties": [
            {
              "errors": [],
              "id": "name",
              "links": [],
              "title": "Name",
              "type": "string",
              "value": "Joe"
            },
            {
              "errors": [],
              "id": "age",
              "links": [],
              "title": "Age",
              "type": "number",
              "value": 7
            }
          ],
          "type": "object"
        },
        {
          "errors": [],
          "links": [],
          "properties": [
            {
              "errors": [],
              "id": "name",
              "links": [],
              "type": "string",
              "value": "Jane"
            },
            {
              "errors": [],
              "id": "age",
              "links": [],
              "type": "number",
              "value": 4
            }
          ],
          "type": "object"
        }
      ],
      "id": "children",
      "links": [],
      "title": "Children",
      "type": "array"
    }
  ]
}
```
