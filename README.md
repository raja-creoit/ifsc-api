# ifsc-api

API server that serves Razorpay's IFSC API.
Current API Root is https://ifsc-api.herokuapp.com/

Routes:

|Route|Method|Response|
|-----|------|--------|
|/:ifsc|GET|JSON|

A sample response is:

```json
{
  "BANK": "KARNATAKA BANK LIMITED",
  "IFSC": "KARB0000001",
  "MICR": "NA",
  "BRANCH": "RTGS-HO",
  "ADDRESS": 2228222,
  "CONTACT": "REGD. & HEAD OFFICE, P.B.NO.599, MAHAVEER CIRCLE, KANKANADY, MANGALORE - 575002",
  "CITY": "MANGALORE",
  "DISTRICT": "DAKSHINA KANNADA",
  "STATE": "KARNATAKA"
}
```

URL: https://ifsc-api.herokuapp.com/KARB0000001
You can see a permalink version of the request [here](http://hurl.eu/hurls/e1d4d8d04d804d72a7506009d19cab583b6549e6/192c7eda180f9537d47e0abe8f7b7c7fa4b419db)

For an invalid IFSC code a 404 is returned.