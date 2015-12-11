## Paths
### Get host info
```
GET /v1/agents/{hostName }
```

#### Description

Returns a list of objects with host info for specified host name

#### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|hostName||true|string||


#### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|AgentBean|


#### Consumes

* application/json

#### Produces

* application/json

#### Tags

* agents

