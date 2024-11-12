sequenceDiagram
    participant browser
    participant server

     Note right of browser: The new note is added to the local array of notes and the page
     Note right of browser: is rendered again with the new note
     browser->>server: POST: https://studies.cs.helsinki.fi/exampleapp/new_note_spa
     server-->>browser: Status code 201 (Created)
    

   