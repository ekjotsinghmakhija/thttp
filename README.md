# tHttp

tHttp is a powerful command-line tool that runs **HTTP requests** defined in a simple, human-readable **plain text format**.

It allows you to chain requests, capture variables, and run complex assertions on headers and response bodies. Whether you are fetching data, testing REST/SOAP/GraphQL APIs, or automation-testing HTML content, tHttp provides a lightweight and fast alternative to complex testing suites.



## Features
- **Fast & Reliable:** Built in Rust on top of libcurl.
- **Text-Based:** Define your API tests in `.thttp` files.
- **Assertions:** Built-in support for JSONPath, XPath, and Regex predicates.
- **Captures:** Chain requests by passing data from one response to the next request.

## Author
**Ekjot Singh**
- 📧 Email: [ekjotmakhija@gmail.com](mailto:ekjotmakhija@gmail.com)
- 🐙 GitHub: [@ekjotsinghmakhija](https://github.com/ekjotsinghmakhija)
- 🔗 LinkedIn: [Ekjot Singh](https://www.linkedin.com/in/ekjot-singh-153110268/)

## Quick Start
Create a file named `get_user.thttp`:
```thttp
GET [https://api.github.com/users/ekjotsinghmakhija](https://api.github.com/users/ekjotsinghmakhija)
HTTP 200
[Asserts]
jsonpath "$.login" == "ekjotsinghmakhija"
```

## Run it
``` bash
thttp get_user.thttp
```

## Installation
Build from source using Cargo:
```bash
cargo build --release
```


