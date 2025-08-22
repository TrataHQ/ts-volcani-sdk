# SidebarSessionsResponse

Response model for sidebar sessions.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **string** | User identifier | [default to undefined]
**sessions** | [**Array&lt;SidebarSession&gt;**](SidebarSession.md) | List of sessions for sidebar | [default to undefined]
**total_sessions** | **number** | Total number of sessions available | [default to undefined]
**has_more** | **boolean** | Whether there are more sessions available | [default to undefined]
**pagination** | **{ [key: string]: any; }** | Pagination information | [default to undefined]

## Example

```typescript
import { SidebarSessionsResponse } from '@trata/ts-volcani-sdk';

const instance: SidebarSessionsResponse = {
    user_id,
    sessions,
    total_sessions,
    has_more,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
