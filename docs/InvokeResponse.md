# InvokeResponse

Response model for agent invocation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**session_id** | **string** | Session identifier | [default to undefined]
**blocks** | [**Array&lt;Block&gt;**](Block.md) | List of blocks with type and content | [default to undefined]
**user_context** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { InvokeResponse } from '@trata/ts-volcani-sdk';

const instance: InvokeResponse = {
    session_id,
    blocks,
    user_context,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
