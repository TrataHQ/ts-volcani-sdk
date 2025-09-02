# ChatSession

Session data for sidebar display.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**session_id** | **string** | Session identifier | [default to undefined]
**name** | **string** | Session name (generated from first message) | [default to undefined]
**user_id** | **string** | User identifier | [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**message_count** | **number** | Number of messages in the session | [default to undefined]
**last_message_preview** | **string** | Preview of the last message | [default to undefined]

## Example

```typescript
import { ChatSession } from '@trata/ts-volcani-sdk';

const instance: ChatSession = {
    session_id,
    name,
    user_id,
    created_at,
    updated_at,
    message_count,
    last_message_preview,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
