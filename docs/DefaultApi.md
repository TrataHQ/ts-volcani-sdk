# DefaultApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getFaviconFaviconIcoGet**](#getfaviconfaviconicoget) | **GET** /favicon.ico | Get Favicon|
|[**getSessionMessagesApiSessionsSessionIdMessagesGet**](#getsessionmessagesapisessionssessionidmessagesget) | **GET** /api/sessions/{session_id}/messages | Get Session Messages|
|[**getStatusStatusGet**](#getstatusstatusget) | **GET** /status | Get Status|
|[**getUserSessionsApiSessionsGet**](#getusersessionsapisessionsget) | **GET** /api/sessions | Get User Sessions|
|[**healthCheckHealthGet**](#healthcheckhealthget) | **GET** /health | Health Check|
|[**invokeAgentInvokePost**](#invokeagentinvokepost) | **POST** /invoke | Invoke Agent|
|[**readRootGet**](#readrootget) | **GET** / | Read Root|
|[**serveUiUiGet**](#serveuiuiget) | **GET** /ui | Serve Ui|

# **getFaviconFaviconIcoGet**
> any getFaviconFaviconIcoGet()

Serve favicon.ico to prevent 404 errors.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.getFaviconFaviconIcoGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSessionMessagesApiSessionsSessionIdMessagesGet**
> SessionMessagesResponse getSessionMessagesApiSessionsSessionIdMessagesGet()

Get all messages for a specific session.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

let sessionId: string; // (default to undefined)

const { status, data } = await apiInstance.getSessionMessagesApiSessionsSessionIdMessagesGet(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**SessionMessagesResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getStatusStatusGet**
> any getStatusStatusGet()

Get the current status of the agent.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.getStatusStatusGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserSessionsApiSessionsGet**
> SidebarSessionsResponse getUserSessionsApiSessionsGet()

Get sessions for sidebar with names and message counts.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

let limit: number; // (optional) (default to 20)
let offset: number; // (optional) (default to 0)

const { status, data } = await apiInstance.getUserSessionsApiSessionsGet(
    limit,
    offset
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **limit** | [**number**] |  | (optional) defaults to 20|
| **offset** | [**number**] |  | (optional) defaults to 0|


### Return type

**SidebarSessionsResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **healthCheckHealthGet**
> any healthCheckHealthGet()

Health check endpoint that doesn\'t require authentication.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.healthCheckHealthGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **invokeAgentInvokePost**
> InvokeResponse invokeAgentInvokePost(invokeRequest)

Invoke the deployed agent with a natural language query.

### Example

```typescript
import {
    DefaultApi,
    Configuration,
    InvokeRequest
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

let invokeRequest: InvokeRequest; //
let accept: string; // (optional) (default to 'application/json')

const { status, data } = await apiInstance.invokeAgentInvokePost(
    invokeRequest,
    accept
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **invokeRequest** | **InvokeRequest**|  | |
| **accept** | [**string**] |  | (optional) defaults to 'application/json'|


### Return type

**InvokeResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **readRootGet**
> any readRootGet()

Health check endpoint for Cloud Run.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.readRootGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **serveUiUiGet**
> any serveUiUiGet()

Serve the main Volcani chat interface.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from '@trata/ts-client-sdk';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.serveUiUiGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

