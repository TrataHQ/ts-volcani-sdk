# ToolCallResponseContent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tool_call_id** | **string** | ID of the tool call | [default to undefined]
**name** | **string** | Name of the tool call | [default to undefined]
**result_content** | **{ [key: string]: any; }** | Result content of the tool call | [default to undefined]
**is_tool_call_error** | **boolean** | Whether the tool call failed | [default to undefined]
**total_response_time** | **number** | Time taken to call the tool | [default to undefined]

## Example

```typescript
import { ToolCallResponseContent } from '@trata/ts-volcani-sdk';

const instance: ToolCallResponseContent = {
    tool_call_id,
    name,
    result_content,
    is_tool_call_error,
    total_response_time,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
