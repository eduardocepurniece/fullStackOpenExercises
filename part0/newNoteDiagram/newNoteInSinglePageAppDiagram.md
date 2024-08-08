sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    browser-->>server: The new_note form json to JS file
    deactivate server

    Note right of browser: The new note appears because of the code in the JS file.