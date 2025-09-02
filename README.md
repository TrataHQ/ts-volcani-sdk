## @trata/ts-volcani-sdk@1.0.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @trata/ts-volcani-sdk@1.0.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**getSessionMessagesApiSessionsSessionIdMessagesGet**](docs/DefaultApi.md#getsessionmessagesapisessionssessionidmessagesget) | **GET** /api/sessions/{session_id}/messages | Get Session Messages
*DefaultApi* | [**getStatusStatusGet**](docs/DefaultApi.md#getstatusstatusget) | **GET** /status | Get Status
*DefaultApi* | [**getUserSessionsApiSessionsGet**](docs/DefaultApi.md#getusersessionsapisessionsget) | **GET** /api/sessions | Get User Sessions
*DefaultApi* | [**healthCheckHealthGet**](docs/DefaultApi.md#healthcheckhealthget) | **GET** /health | Health Check
*DefaultApi* | [**invokeAgentInvokePost**](docs/DefaultApi.md#invokeagentinvokepost) | **POST** /invoke | Invoke Agent


### Documentation For Models

 - [Args](docs/Args.md)
 - [Block](docs/Block.md)
 - [BlockSchema](docs/BlockSchema.md)
 - [ChatMessage](docs/ChatMessage.md)
 - [ChatMessagesResponse](docs/ChatMessagesResponse.md)
 - [ChatSession](docs/ChatSession.md)
 - [ChatSessionResponse](docs/ChatSessionResponse.md)
 - [Content](docs/Content.md)
 - [HTTPValidationError](docs/HTTPValidationError.md)
 - [InvokeRequest](docs/InvokeRequest.md)
 - [InvokeResponse](docs/InvokeResponse.md)
 - [LocationInner](docs/LocationInner.md)
 - [ToolCallRequestContent](docs/ToolCallRequestContent.md)
 - [ToolCallResponseContent](docs/ToolCallResponseContent.md)
 - [ValidationError](docs/ValidationError.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="HTTPBearer"></a>
### HTTPBearer

- **Type**: Bearer authentication

