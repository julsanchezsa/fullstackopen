sequenceDiagram
    participant browser
    participant server

    Note right of browser: JavaScript prevents default form submission, save the info update the UI
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created
    deactivate server
