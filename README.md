# ![LOGO](logo.png) ApiManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the ApiManagementClient API (version 2018-06-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/apimanagement-apimversionsets/2018-06-01-preview/swagger.json<br/>
Generated at: 2019-06-11T18:13:17+03:00

## API Description

Use these REST APIs for performing operations on the ApiVersionSet entity associated with your Azure API Management deployment. Using this entity you create and manage API Version Sets that are used to group APIs for consistent versioning.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists a collection of API Version Sets in the specified service instance.

*Tags:* `ApiVersionSets`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `$filter` - _optional_ - | Field            | Supported operators    | Supported functions               |
|------------------|------------------------|-----------------------------------|
| id               | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
| firstName        | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
| lastName         | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
| email            | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
| state            | eq                     | N/A                               |
| registrationDate | ge, le, eq, ne, gt, lt | N/A                               |
| note             | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
* `$top` - _optional_ - Number of records to return.
* `$skip` - _optional_ - Number of records to skip.

### Deletes specific Api Version Set.

*Tags:* `ApiVersionSets`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `versionSetId` - _required_ - Api Version Set identifier. Must be unique in the current API Management service instance.
* `If-Match` - _required_ - ETag of the Entity. ETag should match the current entity state from the header response of the GET request or it should be * for unconditional update.

### Gets the details of the Api Version Set specified by its identifier.

*Tags:* `ApiVersionSets`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `versionSetId` - _required_ - Api Version Set identifier. Must be unique in the current API Management service instance.

### Gets the entity state (Etag) version of the Api Version Set specified by its identifier.

*Tags:* `ApiVersionSets`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `versionSetId` - _required_ - Api Version Set identifier. Must be unique in the current API Management service instance.

### Updates the details of the Api VersionSet specified by its identifier.

*Tags:* `ApiVersionSets`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `versionSetId` - _required_ - Api Version Set identifier. Must be unique in the current API Management service instance.
* `If-Match` - _required_ - ETag of the Entity. ETag should match the current entity state from the header response of the GET request or it should be * for unconditional update.

### Creates or Updates a Api Version Set.

*Tags:* `ApiVersionSets`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `versionSetId` - _required_ - Api Version Set identifier. Must be unique in the current API Management service instance.
* `If-Match` - _optional_ - ETag of the Entity. Not required when creating an entity, but required when updating an entity.

## License

**flow**ground :- Telekom iPaaS / azure-com-apimanagement-apimversionsets-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
