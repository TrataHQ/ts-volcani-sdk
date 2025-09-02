# ToolCallRequestContent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tool_call_id** | **string** | ID of the tool call | [default to undefined]
**name** | **string** | Name of the tool call | [default to undefined]
**args** | [**Args**](Args.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ToolCallRequestContent } from '@trata/ts-volcani-sdk';

const instance: ToolCallRequestContent = {
    tool_call_id,
    name,
    args,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
