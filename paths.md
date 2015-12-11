## Resources
### Script Tokens
#### Create a system wide script token.
```
POST /v1/system/token_roles
```

##### Description

Creates a specified system wide script token and returns a Response object.

##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Get system token's roles info for a given script name.
```
GET /v1/system/token_roles/{scriptName }
```

##### Description

Returns a TokenRolesBean object containing info about a specified script token.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|scriptName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|TokenRolesBean|


##### Consumes

* application/json

##### Produces

* application/json

#### Update a system wide token's roles.
```
PUT /v1/system/token_roles/{scriptName }
```

##### Description

Updates a specified token's roles given a script name and TokenRolesBean object.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|scriptName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Delete a system wide script token.
```
DELETE /v1/system/token_roles/{scriptName }
```

##### Description

Deletes a system wide script token by specified script name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|scriptName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Get an environment token's roles info for a given environment name and script name.
```
GET /v1/envs/{envName }/token_roles/{scriptName }
```

##### Description

Returns a TokenRolesBean object containing info about a specified script token.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||
|PathParameter|scriptName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|TokenRolesBean|


##### Consumes

* application/json

##### Produces

* application/json

#### Update a specified environment's script token.
```
PUT /v1/envs/{envName }/token_roles/{scriptName }
```

##### Description

Update a specific environment script token specified by environment and script names.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||
|PathParameter|scriptName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Delete an environment script token.
```
DELETE /v1/envs/{envName }/token_roles/{scriptName }
```

##### Description

Deletes a environment name and script name specified script token.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||
|PathParameter|scriptName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Get environment token's roles info for a given environment name.
```
GET /v1/envs/{envName }/token_roles
```

##### Description

Returns a list of the specified environment's TokenRolesBean objects.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|TokenRolesBean array|


##### Consumes

* application/json

##### Produces

* application/json

#### Create an environment script token.
```
POST /v1/envs/{envName }/token_roles
```

##### Description

Creates an environment script token with specified environment name and TokenRolesBean object.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

### User Roles
#### Get user role by user and environment name.
```
GET /v1/envs/{envName }/user_roles/{userName }
```

##### Description

Returns a UserRolesBean object containing info for the specified user and environment name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||
|PathParameter|userName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|UserRolesBean|


##### Consumes

* application/json

##### Produces

* application/json

#### Update a user's role for an environment.
```
PUT /v1/envs/{envName }/user_roles/{userName }
```

##### Description

Updates a UserRolesBean for specified user and environment name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||
|PathParameter|userName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|UserRolesBean|


##### Consumes

* application/json

##### Produces

* application/json

#### Deletes a user from an environment.
```
DELETE /v1/envs/{envName }/user_roles/{userName }
```

##### Description

Deletes a UserRolesBean by specified user and environment name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||
|PathParameter|userName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Get all system level user role objects.
```
GET /v1/system/user_roles
```

##### Description

Returns a list of all system level UserRolesBeans objects.

##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|UserRolesBean array|


##### Consumes

* application/json

##### Produces

* application/json

#### Create a new system level user.
```
POST /v1/system/user_roles
```

##### Description

Creates a system level user specified by UserRolesBean object.

##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Get all user roles for specified environment.
```
GET /v1/envs/{envName }/user_roles
```

##### Description

Returns a list of UserRolesBeans for the specified environment name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|UserRolesBean array|


##### Consumes

* application/json

##### Produces

* application/json

#### Create a user for an environment.
```
POST /v1/envs/{envName }/user_roles
```

##### Description

Creates a new UserRolesBean for a specified environment name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|envName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

#### Get system level user role objects by user name.
```
GET /v1/system/user_roles/{userName }
```

##### Description

Returns a system level UserRolesBean object containing info for the specified user name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|userName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|UserRolesBean|


##### Consumes

* application/json

##### Produces

* application/json

#### Update a system level user's role.
```
PUT /v1/system/user_roles/{userName }
```

##### Description

Updates a system level user's role by specified user name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|userName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|UserRolesBean|


##### Consumes

* application/json

##### Produces

* application/json

#### Deletes a system level user.
```
DELETE /v1/system/user_roles/{userName }
```

##### Description

Deletes a system level user based on specified user name.

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|userName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|default|successful operation|No Content|


##### Consumes

* application/json

##### Produces

* application/json

### Agents
#### Get host info
```
GET /v1/agents/{hostName }
```

##### Description

Returns a list of objects with host info for specified host name

##### Parameters
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|hostName||true|string||


##### Responses
|HTTP Code|Description|Schema|
|----|----|----|
|200|successful operation|AgentBean array|


##### Consumes

* application/json

##### Produces

* application/json

