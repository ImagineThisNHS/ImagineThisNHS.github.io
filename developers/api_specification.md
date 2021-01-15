# API Documentation

## Conversion endpoints


## Feedback endpoints
### List all feedback for given project
- **Method**: ``GET``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback``
- **Request**: N/A
- **Response**:
```json
{
    "project_id": "LgWqYTZMdjG26oA1CxbWaE",
    "feedback": [
        {
            "feedback_id": "123e4567-e89b-12d3-a456-426652340000",
            "project_id": "LgWqYTZMdjG26oA1CxbWaE",
            "upvotes": 7,
            "downvotes": 4,
            "author": "John Dow",
            "timestamp": 1610712842,
            "content": "Great prototype! I would just change the font of the sidebar."
        }
    ] 
}
```

### Get details about a specific feedback
- **Method**: ``GET``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback/{feedback-id}``
- **Request**: N/A
- **Response**:
```json
{
    "feedback_id": "123e4567-e89b-12d3-a456-426652340000",
    "project_id": "LgWqYTZMdjG26oA1CxbWaE",
    "upvotes": 7,
    "downvotes": 4,
    "author": "John Dow",
    "timestamp": 1610712842,
    "content": "Great prototype! I would just change the font of the sidebar."
}
```

### Create a new feedback for a project
- **Method**: ``POST``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback``
- **Request**:
```json
{
    "author": "Elena Hedwick",
    "content": "I don't like the background color of the theme. Too dark."
}
```
- **Response**:
```json
{
    "success": true
}
```

### Vote on existing feedback
- **Method**: ``POST``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback/{feedback-id}/vote``
- **Request**:
```json
{
    "vote": 1
}
```
```warning
The value of the "vote" parameter can be 1 (upvote) or -1 (downvote). All other values are ignored.
```
- **Response**:
```json
{
    "success": true
}
```
