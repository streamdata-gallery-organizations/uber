{
  "info": {
    "name": "Uber User Profile",
    "_postman_id": "2f246ec6-d100-42c4-ad89-0de972dc4d1e",
    "description": "The User Profile endpoint returns information about the Uber user that has authorized with the application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transportation",
      "item": [
        {
          "id": "38183ccc-0204-4f52-b91a-e88484aff69e",
          "name": "the-user-profile-endpoint-returns-information-about-the-uber-user-that-has-authorized-with-the-appli",
          "request": {
            "url": "http://api.uber.com/v1/me",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The User Profile endpoint returns information about the Uber user that has authorized with the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e49d174a-3d43-4b61-98fb-ca963f30b099"
            }
          ]
        }
      ]
    }
  ]
}