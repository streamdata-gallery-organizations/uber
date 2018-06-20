{
  "info": {
    "name": "Uber Product Types",
    "_postman_id": "4cfaa7b7-b0b2-4045-9096-8064c60478a4",
    "description": "The Products endpoint returns information about the Uber products offered at a given location. The response includes the display name and other details about each product, and lists the products in the proper display order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transportation",
      "item": [
        {
          "id": "93e1f16b-2e8f-4374-b845-9c7fd11dd53e",
          "name": "the-products-endpoint-returns-information-about-the-uber-products-offered-at-a-given-location-the-re",
          "request": {
            "url": "http://api.uber.com/v1/products?latitude=%7B%7D&longitude=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Products endpoint returns information about the Uber products offered at a given location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f74183c2-2312-478a-86c2-817bc6aeda8f"
            }
          ]
        }
      ]
    }
  ]
}