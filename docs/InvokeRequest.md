# InvokeRequest

Request model for agent invocation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **string** | Natural language query | [default to undefined]
**session_id** | **string** |  | [optional] [default to undefined]
**client_capabilities** | [**Array&lt;BlockSchema&gt;**](BlockSchema.md) |  | [optional] [default to undefined]

## Example

```typescript
import { InvokeRequest } from '@trata/ts-volcani-sdk';

const instance: InvokeRequest = {
    query,
    session_id,
    client_capabilities,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
