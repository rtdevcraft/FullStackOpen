```mermaid
sequenceDiagram
participant browser
participant server

browser-->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
activate server
server-->>browser: 201 Created
deactivate server

Note right of browser: The POST request contains the new note as JSON data, the server does not redirect and the browser does not send additional HTTP requests
```
