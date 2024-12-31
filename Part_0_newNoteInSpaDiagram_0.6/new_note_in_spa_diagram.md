# Part 0 Exercise 0.6, New note in Single page app diagram

```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: {{"content": "the finale", "date": "2024-12-31T01:46:40.529Z"}, ... }
    deactivate server

    Note right of browser: The single page app doesn't require the entire page to reload and instead, references the HTML form element by fetching the js code from the server instead.
```