# BlockSchema

Schema definition for a block type.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the block | [default to undefined]
**type** | **string** | Block type identifier | [default to undefined]
**description** | **string** | Description of what the block does | [default to undefined]
**data_schema** | **{ [key: string]: any; }** | JSON Schema for expected data to render the block | [default to undefined]

## Example

```typescript
import { BlockSchema } from '@trata/ts-volcani-sdk';

const instance: BlockSchema = {
    name,
    type,
    description,
    data_schema,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
