# API Documentation
This is the list of available endpoints with examples of requests and responses.

## Conversion endpoints

### Authentication

- **Method**: ``GET``
- **Endpoint**: ``/authToken?projectID=&accessToken=&authType=``
- **Request**:  N/A

- **Response**: 

```json
{
    "projectName": "Untitled",
    "wireframeList": ["list", "of", "wireframes"]
}
```

### Generate page

- **Method**: `POST`
- **Endpoint**: ``/generatePage``
- **Request**: 

```json
{
    "accessToken": "153903-bbf3fe57-22dd-4727-bd85-64fd5aed8509",
    "projectID": "LgWqYTZMdjG26oA1CxbWaE",
    "type": "originalToken/oauth2Token",
    "nameList": ["list", "of", "wireframes"]
}
```

- **Response**:

```json
{
    "isSuccess": true,
    "fileName": "OutputStorage/LgWqYTZMdjG26oA1CxbWaE.zip"
}
```

### Download generated prototype

- **Method**: ``GET``
- **Endpoint**: ``/downloadFile?fileName=``
- **Request**: N/A
- **Response**: N/A


## Feedback endpoints (Not implemented yet)
### List all feedback for given project (Not implemented yet)
- **Method**: ``GET``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback``
- **Request**: N/A
- **Response**:
```json
{
    "project_id": "LgWqYTZMdjG26oA1CxbWaE",
    "feedback": [
        {
            "feedback_id": "a843f8df-5c72-4ddd-b300-3e001ae883f9",
            "project_id": "FgWqYTZMdjG26oA1CxbWad",
            "upvotes": 7,
            "downvotes": 4,
            "user_id": "e58adba8-7ce1-435b-9cc1-a35c9c3fbc41",
            "user_name": "Barbara Smith",
            "timestamp": 1610712842,
            "text": "The Click button on the main page didn't work for me."
        }
    ] 
}
```

### Get details about a specific feedback (Not implemented yet)
- **Method**: ``GET``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback/{feedback-id}``
- **Request**: N/A
- **Response**:
```json
{
    "feedback_id": "250a8d14-55d9-4cb1-93e2-29cd4ebda98b",
    "project_id": "MgWqYTZMdjG26oA1CxbWaE",
    "upvotes": 3,
    "downvotes": 0,
    "user_id": "f2366a7b-c2ca-40d5-939a-2f649411d257",
    "user_name": "John Dow",
    "timestamp": 1610955210,
    "text": "Great prototype! I would just change the font of the sidebar."
}
```

### Create a new feedback for a project (Not implemented yet)
- **Method**: ``POST``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback``
- **Request**:
```json
{
    "user_id": "1c93de5b-fff9-4a2f-b702-0214d0b49683",
    "user_name": "Elena Hedwick",
    "text": "I don't like the background color of the theme. Too dark."
}
```
- **Response**:
```json
{
    "success": true
}
```

### Vote on existing feedback (Not implemented yet)
- **Method**: ``POST``
- **Endpoint**: ``/api/v1/projects/{project-id}/feedback/{feedback-id}/vote``
- **Request**:
```json
{
    "user_id": "b84b51ed-8973-4811-8d37-fb1135314782",
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
