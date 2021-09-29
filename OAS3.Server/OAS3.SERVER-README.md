<a name='assembly'></a>
# OAS3.Server

## Contents

- [Body](#T-OAS3-Server-Controllers-Generated-Body 'OAS3.Server.Controllers.Generated.Body')
  - [Name](#P-OAS3-Server-Controllers-Generated-Body-Name 'OAS3.Server.Controllers.Generated.Body.Name')
  - [Status](#P-OAS3-Server-Controllers-Generated-Body-Status 'OAS3.Server.Controllers.Generated.Body.Status')
- [Order](#T-OAS3-Server-Controllers-Generated-Order 'OAS3.Server.Controllers.Generated.Order')
  - [Status](#P-OAS3-Server-Controllers-Generated-Order-Status 'OAS3.Server.Controllers.Generated.Order.Status')
- [Pet](#T-OAS3-Server-Controllers-Generated-Pet 'OAS3.Server.Controllers.Generated.Pet')
  - [Status](#P-OAS3-Server-Controllers-Generated-Pet-Status 'OAS3.Server.Controllers.Generated.Pet.Status')
- [PetControllerBase](#T-OAS3-Server-Controllers-Generated-PetControllerBase 'OAS3.Server.Controllers.Generated.PetControllerBase')
  - [AddPet(body)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-AddPet-OAS3-Server-Controllers-Generated-Pet- 'OAS3.Server.Controllers.Generated.PetControllerBase.AddPet(OAS3.Server.Controllers.Generated.Pet)')
  - [DeletePet(petId)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-DeletePet-System-String,System-Int64- 'OAS3.Server.Controllers.Generated.PetControllerBase.DeletePet(System.String,System.Int64)')
  - [FindPetsByStatus(status)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-FindPetsByStatus-System-Collections-Generic-IEnumerable{OAS3-Server-Controllers-Generated-Anonymous}- 'OAS3.Server.Controllers.Generated.PetControllerBase.FindPetsByStatus(System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.Anonymous})')
  - [FindPetsByTags(tags)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-FindPetsByTags-System-Collections-Generic-IEnumerable{System-String}- 'OAS3.Server.Controllers.Generated.PetControllerBase.FindPetsByTags(System.Collections.Generic.IEnumerable{System.String})')
  - [GetPetById(petId)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-GetPetById-System-Int64- 'OAS3.Server.Controllers.Generated.PetControllerBase.GetPetById(System.Int64)')
  - [UpdatePet(body)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-UpdatePet-OAS3-Server-Controllers-Generated-Pet- 'OAS3.Server.Controllers.Generated.PetControllerBase.UpdatePet(OAS3.Server.Controllers.Generated.Pet)')
  - [UpdatePetWithForm(petId)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-UpdatePetWithForm-System-Int64,OAS3-Server-Controllers-Generated-Body- 'OAS3.Server.Controllers.Generated.PetControllerBase.UpdatePetWithForm(System.Int64,OAS3.Server.Controllers.Generated.Body)')
  - [UploadFile(petId)](#M-OAS3-Server-Controllers-Generated-PetControllerBase-UploadFile-System-Int64,System-String,OAS3-Server-Controllers-Generated-FileParameter- 'OAS3.Server.Controllers.Generated.PetControllerBase.UploadFile(System.Int64,System.String,OAS3.Server.Controllers.Generated.FileParameter)')
- [StoreControllerBase](#T-OAS3-Server-Controllers-Generated-StoreControllerBase 'OAS3.Server.Controllers.Generated.StoreControllerBase')
  - [DeleteOrder(orderId)](#M-OAS3-Server-Controllers-Generated-StoreControllerBase-DeleteOrder-System-Int64- 'OAS3.Server.Controllers.Generated.StoreControllerBase.DeleteOrder(System.Int64)')
  - [GetInventory()](#M-OAS3-Server-Controllers-Generated-StoreControllerBase-GetInventory 'OAS3.Server.Controllers.Generated.StoreControllerBase.GetInventory')
  - [GetOrderById(orderId)](#M-OAS3-Server-Controllers-Generated-StoreControllerBase-GetOrderById-System-Int64- 'OAS3.Server.Controllers.Generated.StoreControllerBase.GetOrderById(System.Int64)')
  - [PlaceOrder(body)](#M-OAS3-Server-Controllers-Generated-StoreControllerBase-PlaceOrder-OAS3-Server-Controllers-Generated-Order- 'OAS3.Server.Controllers.Generated.StoreControllerBase.PlaceOrder(OAS3.Server.Controllers.Generated.Order)')
- [User](#T-OAS3-Server-Controllers-Generated-User 'OAS3.Server.Controllers.Generated.User')
  - [UserStatus](#P-OAS3-Server-Controllers-Generated-User-UserStatus 'OAS3.Server.Controllers.Generated.User.UserStatus')
- [UserControllerBase](#T-OAS3-Server-Controllers-Generated-UserControllerBase 'OAS3.Server.Controllers.Generated.UserControllerBase')
  - [CreateUser(body)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-CreateUser-OAS3-Server-Controllers-Generated-User- 'OAS3.Server.Controllers.Generated.UserControllerBase.CreateUser(OAS3.Server.Controllers.Generated.User)')
  - [CreateUsersWithArrayInput(body)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-CreateUsersWithArrayInput-System-Collections-Generic-IEnumerable{OAS3-Server-Controllers-Generated-User}- 'OAS3.Server.Controllers.Generated.UserControllerBase.CreateUsersWithArrayInput(System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.User})')
  - [CreateUsersWithListInput(body)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-CreateUsersWithListInput-System-Collections-Generic-IEnumerable{OAS3-Server-Controllers-Generated-User}- 'OAS3.Server.Controllers.Generated.UserControllerBase.CreateUsersWithListInput(System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.User})')
  - [DeleteUser(username)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-DeleteUser-System-String- 'OAS3.Server.Controllers.Generated.UserControllerBase.DeleteUser(System.String)')
  - [GetUserByName(username)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-GetUserByName-System-String- 'OAS3.Server.Controllers.Generated.UserControllerBase.GetUserByName(System.String)')
  - [LoginUser(username,password)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-LoginUser-System-String,System-String- 'OAS3.Server.Controllers.Generated.UserControllerBase.LoginUser(System.String,System.String)')
  - [LogoutUser()](#M-OAS3-Server-Controllers-Generated-UserControllerBase-LogoutUser 'OAS3.Server.Controllers.Generated.UserControllerBase.LogoutUser')
  - [UpdateUser(username,body)](#M-OAS3-Server-Controllers-Generated-UserControllerBase-UpdateUser-System-String,OAS3-Server-Controllers-Generated-User- 'OAS3.Server.Controllers.Generated.UserControllerBase.UpdateUser(System.String,OAS3.Server.Controllers.Generated.User)')

<a name='T-OAS3-Server-Controllers-Generated-Body'></a>
## Body `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='P-OAS3-Server-Controllers-Generated-Body-Name'></a>
### Name `property`

##### Summary

Updated name of the pet

<a name='P-OAS3-Server-Controllers-Generated-Body-Status'></a>
### Status `property`

##### Summary

Updated status of the pet

<a name='T-OAS3-Server-Controllers-Generated-Order'></a>
## Order `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='P-OAS3-Server-Controllers-Generated-Order-Status'></a>
### Status `property`

##### Summary

Order Status

<a name='T-OAS3-Server-Controllers-Generated-Pet'></a>
## Pet `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='P-OAS3-Server-Controllers-Generated-Pet-Status'></a>
### Status `property`

##### Summary

pet status in the store

<a name='T-OAS3-Server-Controllers-Generated-PetControllerBase'></a>
## PetControllerBase `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-AddPet-OAS3-Server-Controllers-Generated-Pet-'></a>
### AddPet(body) `method`

##### Summary

Add a new pet to the store

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| body | [OAS3.Server.Controllers.Generated.Pet](#T-OAS3-Server-Controllers-Generated-Pet 'OAS3.Server.Controllers.Generated.Pet') | Pet object that needs to be added to the store |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-DeletePet-System-String,System-Int64-'></a>
### DeletePet(petId) `method`

##### Summary

Deletes a pet

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| petId | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | Pet id to delete |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-FindPetsByStatus-System-Collections-Generic-IEnumerable{OAS3-Server-Controllers-Generated-Anonymous}-'></a>
### FindPetsByStatus(status) `method`

##### Summary

Finds Pets by status

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| status | [System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.Anonymous}](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.Generic.IEnumerable 'System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.Anonymous}') | Status values that need to be considered for filter |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-FindPetsByTags-System-Collections-Generic-IEnumerable{System-String}-'></a>
### FindPetsByTags(tags) `method`

##### Summary

Finds Pets by tags

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| tags | [System.Collections.Generic.IEnumerable{System.String}](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.Generic.IEnumerable 'System.Collections.Generic.IEnumerable{System.String}') | Tags to filter by |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-GetPetById-System-Int64-'></a>
### GetPetById(petId) `method`

##### Summary

Find pet by ID

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| petId | [System.Int64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int64 'System.Int64') | ID of pet to return |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-UpdatePet-OAS3-Server-Controllers-Generated-Pet-'></a>
### UpdatePet(body) `method`

##### Summary

Update an existing pet

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| body | [OAS3.Server.Controllers.Generated.Pet](#T-OAS3-Server-Controllers-Generated-Pet 'OAS3.Server.Controllers.Generated.Pet') | Pet object that needs to be added to the store |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-UpdatePetWithForm-System-Int64,OAS3-Server-Controllers-Generated-Body-'></a>
### UpdatePetWithForm(petId) `method`

##### Summary

Updates a pet in the store with form data

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| petId | [System.Int64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int64 'System.Int64') | ID of pet that needs to be updated |

<a name='M-OAS3-Server-Controllers-Generated-PetControllerBase-UploadFile-System-Int64,System-String,OAS3-Server-Controllers-Generated-FileParameter-'></a>
### UploadFile(petId) `method`

##### Summary

uploads an image

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| petId | [System.Int64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int64 'System.Int64') | ID of pet to update |

<a name='T-OAS3-Server-Controllers-Generated-StoreControllerBase'></a>
## StoreControllerBase `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='M-OAS3-Server-Controllers-Generated-StoreControllerBase-DeleteOrder-System-Int64-'></a>
### DeleteOrder(orderId) `method`

##### Summary

Delete purchase order by ID

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| orderId | [System.Int64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int64 'System.Int64') | ID of the order that needs to be deleted |

<a name='M-OAS3-Server-Controllers-Generated-StoreControllerBase-GetInventory'></a>
### GetInventory() `method`

##### Summary

Returns pet inventories by status

##### Returns

successful operation

##### Parameters

This method has no parameters.

<a name='M-OAS3-Server-Controllers-Generated-StoreControllerBase-GetOrderById-System-Int64-'></a>
### GetOrderById(orderId) `method`

##### Summary

Find purchase order by ID

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| orderId | [System.Int64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int64 'System.Int64') | ID of pet that needs to be fetched |

<a name='M-OAS3-Server-Controllers-Generated-StoreControllerBase-PlaceOrder-OAS3-Server-Controllers-Generated-Order-'></a>
### PlaceOrder(body) `method`

##### Summary

Place an order for a pet

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| body | [OAS3.Server.Controllers.Generated.Order](#T-OAS3-Server-Controllers-Generated-Order 'OAS3.Server.Controllers.Generated.Order') | order placed for purchasing the pet |

<a name='T-OAS3-Server-Controllers-Generated-User'></a>
## User `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='P-OAS3-Server-Controllers-Generated-User-UserStatus'></a>
### UserStatus `property`

##### Summary

User Status

<a name='T-OAS3-Server-Controllers-Generated-UserControllerBase'></a>
## UserControllerBase `type`

##### Namespace

OAS3.Server.Controllers.Generated

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-CreateUser-OAS3-Server-Controllers-Generated-User-'></a>
### CreateUser(body) `method`

##### Summary

Create user

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| body | [OAS3.Server.Controllers.Generated.User](#T-OAS3-Server-Controllers-Generated-User 'OAS3.Server.Controllers.Generated.User') | Created user object |

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-CreateUsersWithArrayInput-System-Collections-Generic-IEnumerable{OAS3-Server-Controllers-Generated-User}-'></a>
### CreateUsersWithArrayInput(body) `method`

##### Summary

Creates list of users with given input array

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| body | [System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.User}](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.Generic.IEnumerable 'System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.User}') | List of user object |

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-CreateUsersWithListInput-System-Collections-Generic-IEnumerable{OAS3-Server-Controllers-Generated-User}-'></a>
### CreateUsersWithListInput(body) `method`

##### Summary

Creates list of users with given input array

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| body | [System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.User}](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.Generic.IEnumerable 'System.Collections.Generic.IEnumerable{OAS3.Server.Controllers.Generated.User}') | List of user object |

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-DeleteUser-System-String-'></a>
### DeleteUser(username) `method`

##### Summary

Delete user

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| username | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The name that needs to be deleted |

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-GetUserByName-System-String-'></a>
### GetUserByName(username) `method`

##### Summary

Get user by user name

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| username | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The name that needs to be fetched. Use user1 for testing. |

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-LoginUser-System-String,System-String-'></a>
### LoginUser(username,password) `method`

##### Summary

Logs user into the system

##### Returns

successful operation

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| username | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The user name for login |
| password | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The password for login in clear text |

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-LogoutUser'></a>
### LogoutUser() `method`

##### Summary

Logs out current logged in user session

##### Returns

successful operation

##### Parameters

This method has no parameters.

<a name='M-OAS3-Server-Controllers-Generated-UserControllerBase-UpdateUser-System-String,OAS3-Server-Controllers-Generated-User-'></a>
### UpdateUser(username,body) `method`

##### Summary

Updated user

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| username | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | name that need to be updated |
| body | [OAS3.Server.Controllers.Generated.User](#T-OAS3-Server-Controllers-Generated-User 'OAS3.Server.Controllers.Generated.User') | Updated user object |
