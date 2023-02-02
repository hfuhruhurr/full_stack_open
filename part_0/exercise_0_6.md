```mermaid
sequenceDiagram
    participant browser
    participant server
    
    browser->>server:  POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser:  creates new note, appends to existing notes list
    deactivate server

    Note right of browser: The browser rerenders the notes

    browser->>server: 
```