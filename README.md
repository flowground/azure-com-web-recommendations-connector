# ![LOGO](logo.png) Recommendations API Client **flow**ground Connector

## Description

A generated **flow**ground connector for the Recommendations API Client API (version 2018-02-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/web-Recommendations/2018-02-01/swagger.json<br/>
Generated at: 2019-05-07T17:39:24+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### List all recommendations for a subscription.

*Tags:* `Recommendations`

#### Input Parameters
* `featured` - _optional_ - Specify <code>true</code> to return only the most critical recommendations. The default is <code>false</code>, which returns all recommendations.
* `$filter` - _optional_ - Filter is specified by using OData syntax. Example: $filter=channel eq 'Api' or channel eq 'Notification' and startTime eq 2014-01-01T00:00:00Z and endTime eq 2014-12-31T23:59:59Z and timeGrain eq duration'[PT1H|PT1M|P1D]
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Reset all recommendation opt-out settings for a subscription.

*Tags:* `Recommendations`

#### Input Parameters
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Disables the specified rule so it will not apply to a subscription in the future.

*Tags:* `Recommendations`

#### Input Parameters
* `name` - _required_ - Rule name
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Get past recommendations for an app, optionally specified by the time range.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `hostingEnvironmentName` - _required_ - Name of the hosting environment.
* `expiredOnly` - _optional_ - Specify <code>false</code> to return all recommendations. The default is <code>true</code>, which returns only expired recommendations.
* `$filter` - _optional_ - Filter is specified by using OData syntax. Example: $filter=channel eq 'Api' or channel eq 'Notification' and startTime eq 2014-01-01T00:00:00Z and endTime eq 2014-12-31T23:59:59Z and timeGrain eq duration'[PT1H|PT1M|P1D]
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Get all recommendations for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `hostingEnvironmentName` - _required_ - Name of the app.
* `featured` - _optional_ - Specify <code>true</code> to return only the most critical recommendations. The default is <code>false</code>, which returns all recommendations.
* `$filter` - _optional_ - Return only channels specified in the filter. Filter is specified by using OData syntax. Example: $filter=channel eq 'Api' or channel eq 'Notification'
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Disable all recommendations for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `environmentName` - _required_ - Name of the app.
* `hostingEnvironmentName` - _required_
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Reset all recommendation opt-out settings for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `environmentName` - _required_ - Name of the app.
* `hostingEnvironmentName` - _required_
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Get a recommendation rule for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `hostingEnvironmentName` - _required_ - Name of the hosting environment.
* `name` - _required_ - Name of the recommendation.
* `updateSeen` - _optional_ - Specify <code>true</code> to update the last-seen timestamp of the recommendation object.
* `recommendationId` - _optional_ - The GUID of the recommendation object if you query an expired one. You don't need to specify it to query an active entry.
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Disables the specific rule for a web site permanently.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `environmentName` - _required_ - Site name
* `name` - _required_ - Rule name
* `hostingEnvironmentName` - _required_
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Get past recommendations for an app, optionally specified by the time range.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `siteName` - _required_ - Name of the app.
* `expiredOnly` - _optional_ - Specify <code>false</code> to return all recommendations. The default is <code>true</code>, which returns only expired recommendations.
* `$filter` - _optional_ - Filter is specified by using OData syntax. Example: $filter=channel eq 'Api' or channel eq 'Notification' and startTime eq 2014-01-01T00:00:00Z and endTime eq 2014-12-31T23:59:59Z and timeGrain eq duration'[PT1H|PT1M|P1D]
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Get all recommendations for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `siteName` - _required_ - Name of the app.
* `featured` - _optional_ - Specify <code>true</code> to return only the most critical recommendations. The default is <code>false</code>, which returns all recommendations.
* `$filter` - _optional_ - Return only channels specified in the filter. Filter is specified by using OData syntax. Example: $filter=channel eq 'Api' or channel eq 'Notification'
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Disable all recommendations for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `siteName` - _required_ - Name of the app.
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Reset all recommendation opt-out settings for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `siteName` - _required_ - Name of the app.
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Get a recommendation rule for an app.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `siteName` - _required_ - Name of the app.
* `name` - _required_ - Name of the recommendation.
* `updateSeen` - _optional_ - Specify <code>true</code> to update the last-seen timestamp of the recommendation object.
* `recommendationId` - _optional_ - The GUID of the recommendation object if you query an expired one. You don't need to specify it to query an active entry.
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

### Disables the specific rule for a web site permanently.

*Tags:* `Recommendations`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group to which the resource belongs.
* `siteName` - _required_ - Site name
* `name` - _required_ - Rule name
* `subscriptionId` - _required_ - Your Azure subscription ID. This is a GUID-formatted string (e.g. 00000000-0000-0000-0000-000000000000).
* `api-version` - _required_ - API Version

## License

**flow**ground :- Telekom iPaaS / azure-com-web-recommendations-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
