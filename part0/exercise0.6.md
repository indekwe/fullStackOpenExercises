```mermaid
sequenceDiagram
    participant user
    participant browser
    participant server


    user->>browser: note
    user->>browser: click "Save" button
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server

    Note right of browser: the browser renders including the new_note