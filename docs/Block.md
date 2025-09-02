# Block

A block with type and content.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the block | [default to undefined]
**type** | **string** | Type of the block (markdown, component, tool_call_request, tool_call_response, etc.) | [default to undefined]
**content** | [**Content**](Content.md) |  | [default to undefined]
**metadata** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { Block } from '@trata/ts-volcani-sdk';

const instance: Block = {
    id,
    type,
    content,
    metadata,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
