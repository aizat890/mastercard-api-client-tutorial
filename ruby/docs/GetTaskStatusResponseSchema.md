# OpenapiClient::GetTaskStatusResponseSchema

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **response_id** | **String** | Unique identifier for the response.  | [optional] |
| **response_host** | **String** | The host that originated the request. Future calls in the same conversation may be routed to this host.  | [optional] |
| **status** | **String** | The status of the specified task. Must be either &#39;PENDING&#39; (The Task has been recieved and is pending processing), &#39;IN_PROGRESS&#39; (The task is currently in progress), &#39;COMPLETED&#39; (The task was completed successfully) or &#39;FAILED&#39; The task was processed but failed to complete successfully.  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::GetTaskStatusResponseSchema.new(
  response_id: 123456,
  response_host: site2.payment-app-provider.com,
  status: FAILED
)
```

