# Goods list

**URL** : `/api/goods/`

**Method** : `GET`

**Auth required** : NO

**Data**:

`{}`

**Or**
```json
{
  "maker": "DARKSIDE"
}
``` 

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
  "count": 2,
  "list": [
    {
      "id": 1,
      "name": "DARKSIDE Bananapapa",
      "maker": "DARKSIDE",
      "desc": "DARKSIDE Bananapapa - это яркий вкус",
      "size": [50,100,250],
      "price": [100,200,500],
      "set": ["Base","Core","Rare"],
      "available": true,
      "taste": [
        {
          "basic": ["first","second","third"],
          "shades": ["first","second","third"],
          "notes": ["first","second","third"],
          "type": ["first","second","third"]
        }
      ]
    },
    {
      "id": 1,
      "name": "DARKSIDE Bananapapa",
      "maker": "DARKSIDE",
      "desc": "DARKSIDE Bananapapa - это яркий вкус",
      "size": [50,100,250],
      "price": [100,200,500],
      "set": ["Base","Core","Rare"],
      "available": true,
      "taste": [
        {
          "basic": ["first","second","third"],
          "shades": ["first","second","third"],
          "notes": ["first","second","third"],
          "type": ["first","second","third"]
        }
      ]
    }
  ]
}
```

## Error Responses

### 400

**Condition** : the request could not be understood or was missing required parameters.

**Code** : `400 Bad Request `

**Content** : 

```json
{"detail": "Bad Request"}
```


### 401

**Condition** : If auth fail

**Code** : `401 Unauthorized`

**Content** :

```json
{"detail": "You do not have permission to perform this action."}
```
