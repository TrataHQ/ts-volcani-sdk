# ChatMessagesResponse

Response model for session messages.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**session_id** | **string** | Session identifier | [default to undefined]
**user_id** | **string** | User identifier | [default to undefined]
**messages** | [**Array&lt;ChatMessage&gt;**](ChatMessage.md) | List of messages in the session | [default to undefined]
**total_messages** | **number** | Total number of messages in the session | [default to undefined]
**has_more** | **boolean** | Always False - no pagination | [default to undefined]
**pagination** | **{ [key: string]: any; }** | Total message count only | [default to undefined]

## Example

```typescript
import { ChatMessagesResponse } from '@trata/ts-volcani-sdk';

const instance: ChatMessagesResponse = {
    session_id,
    user_id,
    messages,
    total_messages,
    has_more,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
