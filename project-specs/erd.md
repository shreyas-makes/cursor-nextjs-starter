erDiagram
    USER ||--o{ PROMPT : creates
    PROMPT ||--|| IMAGE : generates
    USER {
        int id
        string username
        string email
    }
    PROMPT {
        int id
        int user_id
        string text
        datetime created_at
    }
    IMAGE {
        int id
        int prompt_id
        string url
        datetime generated_at
    }