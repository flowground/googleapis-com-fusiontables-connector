# ![LOGO](logo.png) Fusion Tables **flow**ground Connector

## Description

A generated **flow**ground connector for the Fusion Tables API (version v2).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/fusiontables/v2/swagger.json<br/>
Generated at: 2019-05-23T12:13:24+03:00

## API Description

API for working with Fusion Tables data.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Executes a SQL statement which can be any of <br/>
> - SELECT<br/>
> - SHOW<br/>
> - DESCRIBE

*Tags:* `query`

#### Input Parameters
* `hdrs` - _optional_ - Whether column names are included (in the first row). Default is true.
* `sql` - _required_ - A SQL statement which can be any of 
- SELECT
- SHOW
- DESCRIBE
* `typed` - _optional_ - Whether typed values are returned in the (JSON) response: numbers for numeric values and parsed geometries for KML values. Default is true.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Executes a Fusion Tables SQL statement, which can be any of <br/>
> - SELECT<br/>
> - INSERT<br/>
> - UPDATE<br/>
> - DELETE<br/>
> - SHOW<br/>
> - DESCRIBE<br/>
> - CREATE statement.

*Tags:* `query`

#### Input Parameters
* `hdrs` - _optional_ - Whether column names are included in the first row. Default is true.
* `sql` - _required_ - A Fusion Tables SQL statement, which can be any of 
- SELECT
- INSERT
- UPDATE
- DELETE
- SHOW
- DESCRIBE
- CREATE
* `typed` - _optional_ - Whether typed values are returned in the (JSON) response: numbers for numeric values and parsed geometries for KML values. Default is true.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a list of tables a user owns.

*Tags:* `table`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of tables to return. Default is 5.
* `pageToken` - _optional_ - Continuation token specifying which result page to return.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new table.

*Tags:* `table`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.
    Possible values: csv, json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Imports a new table.

*Tags:* `table`

#### Input Parameters
* `delimiter` - _optional_ - The delimiter used to separate cell values. This can only consist of a single character. Default is ,.
* `encoding` - _optional_ - The encoding of the content. Default is UTF-8. Use auto-detect if you are unsure of the encoding.
* `name` - _required_ - The name to be assigned to the new table.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes a table.

*Tags:* `table`

#### Input Parameters
* `tableId` - _required_ - ID of the table to be deleted.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a specific table by its ID.

*Tags:* `table`

#### Input Parameters
* `tableId` - _required_ - Identifier for the table being requested.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates an existing table. Unless explicitly requested, only the name, description, and attribution will be updated. This method supports patch semantics.

*Tags:* `table`

#### Input Parameters
* `replaceViewDefinition` - _optional_ - Whether the view definition is also updated. The specified view definition replaces the existing one. Only a view can be updated with a new definition.
* `tableId` - _required_ - ID of the table that is being updated.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates an existing table. Unless explicitly requested, only the name, description, and attribution will be updated.

*Tags:* `table`

#### Input Parameters
* `replaceViewDefinition` - _optional_ - Whether the view definition is also updated. The specified view definition replaces the existing one. Only a view can be updated with a new definition.
* `tableId` - _required_ - ID of the table that is being updated.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a list of columns.

*Tags:* `column`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of columns to return. Default is 5.
* `pageToken` - _optional_ - Continuation token specifying which result page to return.
* `tableId` - _required_ - Table whose columns are being listed.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Adds a new column to the table.

*Tags:* `column`

#### Input Parameters
* `tableId` - _required_ - Table for which a new column is being added.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified column.

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column being deleted.
* `tableId` - _required_ - Table from which the column is being deleted.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a specific column by its ID.

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column that is being requested.
* `tableId` - _required_ - Table to which the column belongs.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the name or type of an existing column. This method supports patch semantics.

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column that is being updated.
* `tableId` - _required_ - Table for which the column is being updated.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the name or type of an existing column.

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column that is being updated.
* `tableId` - _required_ - Table for which the column is being updated.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Copies a table.

*Tags:* `table`

#### Input Parameters
* `copyPresentation` - _optional_ - Whether to also copy tabs, styles, and templates. Default is false.
* `tableId` - _required_ - ID of the table that is being copied.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Imports more rows into a table.

*Tags:* `table`

#### Input Parameters
* `delimiter` - _optional_ - The delimiter used to separate cell values. This can only consist of a single character. Default is ,.
* `encoding` - _optional_ - The encoding of the content. Default is UTF-8. Use auto-detect if you are unsure of the encoding.
* `endLine` - _optional_ - The index of the line up to which data will be imported. Default is to import the entire file. If endLine is negative, it is an offset from the end of the file; the imported content will exclude the last endLine lines.
* `isStrict` - _optional_ - Whether the imported CSV must have the same number of values for each row. If false, rows with fewer values will be padded with empty values. Default is true.
* `startLine` - _optional_ - The index of the first line from which to start importing, inclusive. Default is 0.
* `tableId` - _required_ - The table into which new rows are being imported.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Replaces rows of the table with the rows of the spreadsheet that is first imported from. Current rows remain visible until all replacement rows are ready.

*Tags:* `table`

#### Input Parameters
* `tableId` - _required_ - Table whose rows will be replaced from the spreadsheet.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Replaces rows of an existing table. Current rows remain visible until all replacement rows are ready.

*Tags:* `table`

#### Input Parameters
* `delimiter` - _optional_ - The delimiter used to separate cell values. This can only consist of a single character. Default is ,.
* `encoding` - _optional_ - The encoding of the content. Default is UTF-8. Use 'auto-detect' if you are unsure of the encoding.
* `endLine` - _optional_ - The index of the line up to which data will be imported. Default is to import the entire file. If endLine is negative, it is an offset from the end of the file; the imported content will exclude the last endLine lines.
* `isStrict` - _optional_ - Whether the imported CSV must have the same number of column values for each row. If true, throws an exception if the CSV does not have the same number of columns. If false, rows with fewer column values will be padded with empty values. Default is true.
* `startLine` - _optional_ - The index of the first line from which to start importing, inclusive. Default is 0.
* `tableId` - _required_ - Table whose rows will be replaced.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a list of styles.

*Tags:* `style`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of styles to return. Optional. Default is 5.
* `pageToken` - _optional_ - Continuation token specifying which result page to return. Optional.
* `tableId` - _required_ - Table whose styles are being listed
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Adds a new style for the table.

*Tags:* `style`

#### Input Parameters
* `tableId` - _required_ - Table for which a new style is being added
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes a style.

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (within a table) for the style being deleted
* `tableId` - _required_ - Table from which the style is being deleted
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets a specific style.

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (integer) for a specific style in a table
* `tableId` - _required_ - Table to which the requested style belongs
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates an existing style. This method supports patch semantics.

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (within a table) for the style being updated.
* `tableId` - _required_ - Table whose style is being updated.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates an existing style.

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (within a table) for the style being updated.
* `tableId` - _required_ - Table whose style is being updated.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a list of tasks.

*Tags:* `task`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of tasks to return. Default is 5.
* `pageToken` - _optional_ - Continuation token specifying which result page to return.
* `startIndex` - _optional_ - Index of the first result returned in the current page.
* `tableId` - _required_ - Table whose tasks are being listed.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes a specific task by its ID, unless that task has already started running.

*Tags:* `task`

#### Input Parameters
* `tableId` - _required_ - Table from which the task is being deleted.
* `taskId` - _required_ - The identifier of the task to delete.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a specific task by its ID.

*Tags:* `task`

#### Input Parameters
* `tableId` - _required_ - Table to which the task belongs.
* `taskId` - _required_ - The identifier of the task to get.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a list of templates.

*Tags:* `template`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of templates to return. Optional. Default is 5.
* `pageToken` - _optional_ - Continuation token specifying which results page to return. Optional.
* `tableId` - _required_ - Identifier for the table whose templates are being requested
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new template for the table.

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table for which a new template is being created
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes a template

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table from which the template is being deleted
* `templateId` - _required_ - Identifier for the template which is being deleted
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a specific template by its id

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table to which the template belongs
* `templateId` - _required_ - Identifier for the template that is being requested
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates an existing template. This method supports patch semantics.

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table to which the updated template belongs
* `templateId` - _required_ - Identifier for the template that is being updated
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates an existing template

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table to which the updated template belongs
* `templateId` - _required_ - Identifier for the template that is being updated
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-fusiontables-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
