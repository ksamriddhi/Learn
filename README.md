# Learn
DataEngg 
Flattening a File in semi - structure data
Convert nested Json - data organized in multiple layers of objects and arrays to simple flat structure- few levels

Transform complex json objects - arrays into a format which is easy to work with for analysis, storage or processing
Example -
Nested JSON -
{
  "name": "John",
  "address": {
    "street": "123 Elm St",
    "city": "Springfield"
  },
  "contacts": [
    { "type": "email", "value": "john@example.com" },
    { "type": "phone", "value": "123-456-7890" }
  ]
}



Flattened -
{
  "name": "John",
  "address_street": "123 Elm St",

  "address_city": "Springfield",
  "contacts_1_type": "email",
  "contacts_1_value": "john@example.com",
  "contacts_2_type": "phone",
  "contacts_2_value": "123-456-7890"
}
Flattening makes it easier to analyze and query data in databases or other tools that don't handle complex nested structures well
