
# RESTful API

A complete RESTful API following the Richardson Maturity Model.

## Stack

**Back-end:** Java 17, Spring Boot 3, Spring Framework\
**API Tester:** Postman\
**Database:** PostgreSQL


## References

 - [Spring Boot 3 | Complete Course 2023](https://www.youtube.com/watch?v=wlYvA2b1BWI&ab_channel=MichelliBrito)
 - [Spring Boot: Da API REST aos Microservices](https://www.michellibrito.com/so/tr/9594dcca-413b-46f3-a816-2ae8c623b52a/c?w=F3SdWAfGAvDC7zSyFVro9e99upPe7IrAglS3mjc7y78.eyJ1IjoiaHR0cHM6Ly9kZTY3Y2RmOC1kZTkxLTQ1ZGMtODRiMi1jYWZkNDE1ODJmYmQudXNyZmlsZXMuY29tL3VnZC8yMTdlN2JfNGMzNWE5MjRhZWM5NGVhMDlkMzc3OTlmNjM4ZjdkZDEucGRmP2RuPWVib29rLXNwcmluZ2Jvb3QtNGVkaWNhby5wZGYiLCJyIjoiNThiMmI2MjQtYmJiMS00YmQ3LTc5ZTktZjFhMWMyN2FiZTg1IiwiYyI6ImViZDlmMWU5LWU3Y2MtNDFjNi05MTViLTFmNTAxMTA1MDc2NSIsIm0iOiJtYWlsIn0)


## API Methods

- POST
```json
"name": "Monitor Dell 27",
        "value": 4600.00,
```
```json
"name": "Lavadora LG",
        "value": 3500.00
```
```json
"name": "Cadeira Gamer",
        "value": 1500.00
```
- GET ONE
```json
{
    "idProduct": "60db7ad7-7e1f-4c7b-b04d-2a2157af1a3b",
    "name": "Monitor Dell 27",
    "value": 4600.00,
    "_links": {
        "Products list": {
            "href": "http://localhost:8090/products"
        }
    }
}
```
- GET ALL
```json

[
    {
        "idProduct": "60db7ad7-7e1f-4c7b-b04d-2a2157af1a3b",
        "name": "Monitor Dell 27",
        "value": 4600.00,
        "links": [
            {
                "rel": "self",
                "href": "http://localhost:8090/products/60db7ad7-7e1f-4c7b-b04d-2a2157af1a3b"
            }
        ]
    },
    {
        "idProduct": "597f6116-57f5-4c94-af4f-66d7c93ccc18",
        "name": "Lavadora LG",
        "value": 3500.00,
        "links": [
            {
                "rel": "self",
                "href": "http://localhost:8090/products/597f6116-57f5-4c94-af4f-66d7c93ccc18"
            }
        ]
    },
    {
        "idProduct": "0f231ec1-9942-455c-9994-cb6faa00ffdc",
        "name": "Cadeira Gamer",
        "value": 1500.00,
        "links": [
            {
                "rel": "self",
                "href": "http://localhost:8090/products/0f231ec1-9942-455c-9994-cb6faa00ffdc"
            }
        ]
    }
]
```
- UPDATE
```json
ID: 60db7ad7-7e1f-4c7b-b04d-2a2157af1a3b

Before

{
	"name": "Monitor Dell 27",
    "value": 4600.00
}

After

{
	"name": "Monitor Dell 27 ATUALIZADO",
    "value": 55000.00
}
```
- DELETE
```json
ID: 60db7ad7-7e1f-4c7b-b04d-2a2157af1a3b

Product deleted successfully.
```

