# ChatMessage

A single chat message in the conversation history.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **string** | Unique message identifier | [default to undefined]
**session_id** | **string** | Session identifier | [default to undefined]
**timestamp** | **string** | When the message was sent | [default to undefined]
**role** | **string** | Role: \&#39;user\&#39;, \&#39;assistant\&#39;, or \&#39;tool_call\&#39; | [default to undefined]
**content** | **string** | Message content | [default to undefined]
**blocks** | [**Array&lt;Block&gt;**](Block.md) |  | [optional] [default to undefined]
**metadata** | **{ [key: string]: any; }** | Additional message metadata | [optional] [default to undefined]
**tool_name** | **string** |  | [optional] [default to undefined]
**tool_args** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**tool_result** | **string** |  | [optional] [default to undefined]
**tool_error** | **boolean** |  | [optional] [default to undefined]
**type** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ChatMessage } from '@trata/ts-client-sdk';

const instance: ChatMessage = {
    message_id,
    session_id,
    timestamp,
    role,
    content,
    blocks,
    metadata,
    tool_name,
    tool_args,
    tool_result,
    tool_error,
    type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
