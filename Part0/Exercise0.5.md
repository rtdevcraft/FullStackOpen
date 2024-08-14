```mermaid
sequenceDiagram
participant browser
participant server

browser-->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
activate server
server-->>browser: 200 OK
deactivate server

Note right of browser: The browser fetches only one HTML page from the server, which are then manipulated with JavaScript that executes in the broswer
```
