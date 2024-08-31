sequenceDiagram
    participant User
    participant App
    participant ReplicateAPI
    participant Database

    User->>App: Enter text prompt
    App->>ReplicateAPI: Send text prompt
    ReplicateAPI->>ReplicateAPI: Generate image
    ReplicateAPI->>App: Return generated image
    App->>Database: Store prompt and image URL
    App->>User: Display generated image