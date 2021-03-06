---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Activate a customer class
  description: Activates a customer class for a sales price. The ID of the sales price
    and the ID of the customer class must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/classes/{contactClassId}:
    get:
      summary: Get a contact class
      description: Gets a contact class. The ID of the contact class must be specified.
      operationId: getRestAccountsContactsClassesContactclass
      x-api-path-slug: restaccountscontactsclassescontactclassid-get
      parameters:
      - in: path
        name: contactClassId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Class
  /rest/items/sales_prices/{id}/customer_classes:
    post:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: postRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/customer_classes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---