# Documenta2 API Reference

Request path elements
---------------------

<namespace>

<resource_path>

Accessing an existing resource
------------------------------

### Request

GET /api/<namespace>/<resource_path>

### Request body

empty

### Response

| Status | Reason             | Body          |
-----------------------------------------------
| 200    | successful request | resource data |
| 404    | resource not found | empty         |

Creating a new resource
-----------------------

### Request:

POST /api/<namespace>/<resource_path>

### Request body:

data

### Response

| Status | Reason                      | Body                |
--------------------------------------------------------------
| 201    | New resource created        | URL of new resource |
| 404    | Path to resource is invalid | empty               |

Updating an existing resource
-----------------------------

### Request

PUT /api/<namespace>/<resource_path>

### Request body

Resource data

### Response

| Status | Reason                        | Body  | 
--------------------------------------------------
| 204    | Resource updated              | empty | 
| 404    | Path to resource is invalid   | empty |

Deleting an existing resource
-----------------------------

### Request

DELETE /api/<namespace>/<resource_path>

### Request body

empty

### Response

| Status | Reason                      | Body  |
------------------------------------------------
| 200    | Resource has been deleted   | empty |
| 404    | Path to resource is invalid | empty |
